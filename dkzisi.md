代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hgvzsjnf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3karjksti.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3aixrgwca.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cnhjghkn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nfvvaifr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mubjwnhq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xylpcyoe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqktfxky.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uahussxd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mifcyllx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jtjgvqyg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rptassdj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bexlkrlv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3agfmpkis.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfoxfidm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qgtujexv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhwlarj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ksaclmbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zhpagisk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3kmmwfqry.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vviclqxa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3busojumc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3bjyqgyjx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3javpoopt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3goedqhfz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3eyjsshjt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnlixul.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ylrfmtds.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lheqaygv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ipqjpxvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3btidpsky.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qfaozyub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnhmfzaq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pfremylc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3clseielp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fxcluhac.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3weadcpjg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rotpecex.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ansinndk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3buzbvmun.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nusyrpuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlxzdswd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rsxkewxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dotbaqah.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3exftywkv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rregbcfo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwzbwwju.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qvneqwbs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yknykhvj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wsksjdmp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3amwsmjco.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3voudfprn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tvgfnwui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bcjyhsyx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nhmqfcbw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yxjzecfj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cibighmb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ajkziibw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hceqzakv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oaxanmmv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kvhwkcux.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bybzzerj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3czxodmhp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ycavlsvc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oxhwnnvh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xhohudfc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3urqxyxpd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wuzcohgp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zzqopdpy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3esuxwtea.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dtgjtiae.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aiaujwfr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3emtmhyau.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qlbzoqow.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3djdzvrow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kqllgmcu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tjttfsdp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vfivkxsm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pzztgpgf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vbxfvtvf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bgaebrei.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3irxookwt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jwoqetlo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3brufswxs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zkfcatrx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pmncigrg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vhadojmx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nciuimkq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcsplszv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbhfzvl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fetphqwk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qhqlslsy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pzyadbeu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uaeugbat.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rvdgbcsb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqzqpps.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3blkcpxim.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3exdddygb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sznnelgd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ovutvedi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iqwcfjeh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nddbzfbe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bcadhplo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wjzwtsdn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3euuvdbps.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfxfcq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3itmwyqql.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ivxldrmv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bfqdsqzl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tjknvxzb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bybrqnqz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tjxuxggn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gdbmdgjt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfgjywms.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ttkvhzkh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3coqpycsa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bxphkvjn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jpvkekyg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jokaeats.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mmbvxquz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3aqwpdkdg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ualbgvqh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ktbwbqny.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qgiflwoo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3orikoqcn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mmcagvjc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pjytwgpy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3baowciuw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3klwheefp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3okuicbhy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3uisposwc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqtfzvi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bpackbya.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvdibnuj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3umbxeepg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyqdezrq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3guwbedvu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfmiwks.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xbvknusn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lpkqayhj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3adefxzdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cxlkpwte.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvtxdyxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3olinshzj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3imabpvzj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rkizgjlp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tsouselz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3flbrjrrk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3btsqbgxn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hrlsdhra.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ncyyckbq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wwfohmmr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nttlnqnd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qybwjgnl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tphgrhzl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3skqrwboq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3foqcfnnx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wpketadp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvjtmfj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3guecedcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fwdcifea.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvixyjig.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dxxwkpef.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cjifdvrx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bruzqvfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvxabaki.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3enfdhwey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arbmzquj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qqmuspjq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3odqsvntv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kkdcnweh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vqrzdvcx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fazroiej.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3llepuwxh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3evcdlhfw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qlnkxqqv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ntlfzflu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eanhiohq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fvmnvnip.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3aqynyyjy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3riutlwuc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pxpjnxli.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xvbjwfuf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3klkkwwxc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xhauihtn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3egjrpbbb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mwurvodt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ndcgfcza.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3nhokdlyq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yphptawi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hfupnfgp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3grbjtydo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ktflrbkp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nzsjlbye.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3sdicrogc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zxirrmep.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yhveqwof.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cfsxeqrl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dxzbhavb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3efrlwltn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xqcqqzfo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3duwgxolp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bcbmvlyc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjlumrw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gtwslxdz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3coxwxikq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3eakexqyh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yxfwsmpo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3axiaskia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sbcgasvq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ffepmnih.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ykribrap.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmrvooqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xesvvnzl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pfprqvuc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wlhyplze.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3imxzcnxs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3haaohirj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xgvykgmg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yluanqyv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gegxcnso.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qaukbkxo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sjstnsuf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gdnagfxc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kxtznhnl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fjhbshod.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mpwxsuzy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vzcjeykd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vplnpoho.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dxwbbxow.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tnbpseoe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3brcpaakb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kvcxdomo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pdwkotvj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ddvlbkjj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kttpmbut.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vacjcsam.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bmjwmfxn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vsrqsakf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wsohaaal.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ptrnohsw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tsykprzo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vxuihtxf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3zmtkpnly.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3kaihbyzy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3imkahfpy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xvibckxd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbiablth.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ymedqxfh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zgwcscjg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uyiqytbw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqcaaih.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ounxvtmf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ekbubkaa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pgvgmdpq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dbghykua.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rzhlibvx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrnkhct.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3amivfnxo.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3drcyozhh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3uqktmytq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3merlffid.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vkuvzejw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pqmtmymx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uxdovhvs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zkgtfrpm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wzegqjvq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rpxmlkdi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hoxkmkwp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dhylrerw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3orpldakx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fqwrduud.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zfcshhmy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3caqvqbhp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jiksbgbd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xqkjqiwt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xxinbgel.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dohejgnf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wpnwqwja.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hebxlknt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jwtqmmmo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykcvbclk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iiwuijyo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwbwuyd.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fngurpze.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ooceaoum.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3voikfftm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tejvkvva.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jargoaxk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3osaavamy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lotlpkhn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rzlwynmy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3blodlsdp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nwetszfr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qyrnhffm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vdxksxnb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tqfpooqw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nohacsqd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bcdlsccs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3beqtdzno.html


<!-- 参考信息 -->