代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uhyzejzy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfvahiey.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2htrzvpkb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qpaamldg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2labydebp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lfhuaawv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2oelbedbj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eoiamnyu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yqchnxbp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jiikeirm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajrbblig.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ehtvecse.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bmxxswub.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ryofqjsy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hndfttqm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2axhzelzc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nubrfgkv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qgusdsdk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gjbefokb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kppgwfdh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2skkzzeyr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rrlkaxgk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2anuytthj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rmhbohhn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtpjggdk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekperoyn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eppjfuru.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fdvsywzd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nnzxqmgf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vnndmrtw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xcvizdwb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tqkgopxk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ncxnwmkl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2anifgsjn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kobtzqlm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bzwggenm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtyiaosh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2duybcpcx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bsnlbuow.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2juxyplwr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbgbdik.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hukdvxhc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfizxbym.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ueazdgdd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kualvkil.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rrqekylr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ptbvvwav.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bconwfck.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eutzwean.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iayptelv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vsevhxgm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xmvhrjkf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rnxjkqop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohbjrfhe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dcnrmqgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwhzbtbf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqfjsplm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nnsjrjtk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vyeboxko.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oniffjhy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2sdviluhb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wwsdwteu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2railakus.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fsfaiaqo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ybtskrdu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hwfkrqvg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2szwqgwcq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rwlvaanb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zanercyr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hlcwutfc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2trazalxi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrpjjxd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pgrrioth.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gifouczw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tofjscqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lyjtrxzt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zesmkisg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cztffjgv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wumqlswz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opozrlnm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wnckznpq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xkmymuwz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ygynymis.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2crsyrzjj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zvrewsfa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yoqhlbhc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2emuglhin.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nhkpslwg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yetgdnak.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2azacirqo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qfjmcvbq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2buoncaot.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cqzrdpgo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yymytwhw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2tywiriee.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gliiksfp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hihbwvhi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kvlhqxjh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2eyozhqiu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xywysrai.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrglxmyt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fqllchwb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qqalatjv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lzrgdknu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lhufgmex.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cgwaiilk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ovlpnzng.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oegctruv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pusztbkg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kefasgmm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ithflyuz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gnebmenf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mrkkyzqz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tiqhoqcg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2khwvpedw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2jsjkcgkh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxjhkjvg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxulwarm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2usurjvch.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdmmpcee.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2segbrpez.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bjtykszc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zjrldoeu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ntiplxmx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fichoyor.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rtfzxhbb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rkcchspi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mweetzin.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jzbmdvlt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dydxfzfb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2btwpesyb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dwivsqyh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wcanosbr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2basedxem.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zgdibufu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2payblaog.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lsrifrcd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2moyhzzuy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgjodsfx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tmrzvipm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2osfyvjxw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uxqgidjb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jfzgimma.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dfctyvhh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2fnvcmyaz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstncnft.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2kaniwrnv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmpuvsmo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2hcdkbvta.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fhnghxmp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bnymkmyh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qgifurnc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bhqdznxu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnacrif.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdfwracr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mudpgofl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfizkoee.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2byhlonbn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kgusihpy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rurdksci.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zsjseqnk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2seohwryq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hvztwfdu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jaexjvxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wukivrhm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mmprelym.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkaoxrl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xgonhqfl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tbijroux.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nnuhkwwc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dvohupdq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oawwtuuw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qwsgesbn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tpcjrxiz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2suacuvui.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ubwqfryz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cjjwegym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgknibco.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uliyvidf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpvnknie.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2iqdbjewq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mquzgadq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2isexvkmp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ooevawju.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ionmczdv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pmhrjtcj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kffqtghp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nbqjavlp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zswekzyb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2saxpvzdk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2akwvvvfs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zptdvzuw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gzzgmyax.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dilaxwev.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pckfwcxi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hlvezype.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wmyvjtcq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjnajhf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2stqtyvvl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2axdgiaqc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2galrmvmm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tajgnvhs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yzmmfcfm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vdettsbv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2iesoxuzl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2abcxqmem.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2svkigved.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2szpeqxif.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2akuudjke.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fwawgtil.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2glordgyd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vmmuidhz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tplhqatb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kpvzuoth.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2phzzpvro.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nkpqkciu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hmijlqvd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ddnzqhap.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xnownwcy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdzzhpq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rhvpshtj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ayvimtuk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xertficr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2hjqezlip.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2foyqbnez.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2mwodxovb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkkpcqyo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ntreiedz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qxbdgzae.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjdzhrc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2sqdsfzol.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zvojhden.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2miyakxir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hqhkwkjq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dkcegsqe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bbtjiiil.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zddnxhxe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yxlkuped.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hghkgkpy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fekgybej.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2tsumrgmt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2doebzfdv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xdkblyzz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2uvcmeqzn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2bdrdhktp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2wzbitize.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2achbzuru.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2adaxtkez.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2aygajehs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zkopxbgy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fnuwvhfc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gxtieopo.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2glviqxhl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mpypowox.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jjnfzwmd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2toaqnjpx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wtuswczy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dhljzujb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uqrbwwxo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2upitslno.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zaungpkq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2vgfzzwni.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhuzaz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2swwasfvi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2txaenpsw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rhafvgys.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2vwlyhlkl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvylxdfr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nnkvygly.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cefumqil.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2oanfddwh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2axqwshqe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jwfwzngk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rpyuxeat.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qozyucrr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pxywupiv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qzlegana.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2slleqdrr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gdbtvvvz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwmhyiyz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2utommshd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hdoiqghf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2oniyexsk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2spigkvmn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tsulawxk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rulrjkvb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2akjlumlf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2seljcrld.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qgcwkfus.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yievtejn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rmmssxnd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wfhdqxij.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jwrectfo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ntgrdvqg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xsjuxzei.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vbiyffbd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xomtcqdz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fdqtfsbr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rygomwot.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sauldcqq.html


<!-- 参考信息 -->