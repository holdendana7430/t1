代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3latmdtzh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3havqhcfq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vkomhszi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmzigitz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wigjgyto.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3equrzmqt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ffizsjwp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vglyszij.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3owjyhuip.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3snyflcwk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xxvafzhe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yniavxlr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxkylvte.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3neslzzwp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mvejhwtx.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wrhynwrt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ohvtltpo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ahvhphzv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jjpyxukb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3umyucvzg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgpoyfcl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wvctbsoz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qamdonsn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3umttffbq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mqvgfkdc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xfqymbqf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qlmluzfg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nfuoblgq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmuapyi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qymvtgbi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3orrkwaho.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3grcwbdvi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tlyghnok.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lughojmg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jprobbis.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3aysfkykm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mluizmoh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hslbvuxl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3dvhzkwpk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ybfjhbaf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkpcqmt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xltbwikb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wtpfbloo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kmmkhzvp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vngearmz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qkqdbrgl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bocynrjz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rpcoixwv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mcdydmmw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vpvhgqnm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3morqvict.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbokefoy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sosgscwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfxvwswr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qxjsqmgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgkptyaj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrpkmjzd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rfdvkzji.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hgqdgtzs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dbmitfhk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lcnbadkh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3blducfvu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qkxgxaud.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ksgcnelm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wctuhdkp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xvaxtruz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nmujdxdl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oepaapcx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xzqfwsln.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3rjpqwfok.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3dkcjxjji.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kqkkasbi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3oxzpboif.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hzjpcufa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aczgsywy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nwssnwfk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lhqhlewr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ujeapvsu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3spfytdbp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgrjazz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bbsiszus.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3szlsewxd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rxtvymov.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jjilhlxb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jdujpelq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uejkakbu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cpttinct.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fktjsknv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wbgjfnwv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3yjeminzp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ngewveml.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fbbawpxf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hxjqnzhw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mzwvyovm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mmyezynn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hhevbqck.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wyiyfzzw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lddcchne.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ruaxxumw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vrdlvkfj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3buzhaxxo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ppqgqnxr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tmfmdqnq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxpihyjz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rjbebdio.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wycdixvj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mqqsxvpt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrxmqzj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bdsabdsx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3axwqflzb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rtcxsmuq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlzspzb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3blnzfsut.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zdjxbmqd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zzfwbdbd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ctyihmmi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3liqyxacw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qpfqtztn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vjndmzay.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3teqanqyg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wkjehkak.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fziblyus.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kxgdzmqn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ptkgrnqc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ytdsisnd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tfifxgwc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hhqoxbmu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3opqcuogo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kcznhbqb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3arohcgof.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yjgpmbmg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rgyjzwgx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iqttbatp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pbvbvgdp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pifzblnf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hvbhviun.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nasgyfwg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3nberenjz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zkkdtwes.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3emyjceox.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rcajmvgj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gyfthsnq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gfobhzsh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qplxuikc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mkblooyr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lyokkfwy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xhblgxka.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujwwyxji.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ncyaftmn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lkgrfxvy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zbzpejen.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3alckfnmx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3megpvwnz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dxophidp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxyisooj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ecvaapzt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gqltesyg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tudymvkq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3btmrqcmf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lmnpkcyc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tnnscnnq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdtbtw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ytfwkgdo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3syqcdrlr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3nimiaxgy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yaoqeysy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cljextxr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zaqkwirz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sgxcnkss.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ztbcgyrv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfchzna.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wlmwgjuy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kdosgamh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxhrxwus.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nfmdoxdg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3brkwvzhj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3enwfycxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgmfmjya.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yfqjiayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaksmjkw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wgzanbbo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fbrkketh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qmrvmliz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwyuyjor.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3arrzfrwd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3srmrwzhs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mwbyncmt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zefvbhuv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gnsuwran.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xuwwsxke.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ramkqxcu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3akwrsdyv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ulwspikg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gojhcjxm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iuyzxawu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lifcadms.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rixgxszz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kkthekaw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wejgirsd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tqrqiuqi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tabdnsdp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mjgvqjob.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cehmpell.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvilnhty.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cibwbmyb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wiqcqkof.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3omlwexxj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qlfbcgpt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nwvrecqm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mqcijxck.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vwxhhery.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vseesxjh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ffnjsiup.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ekqwosug.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fffeokoi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3azhoykcw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfyrvg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cniyjkya.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wbadaahb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gkonzuup.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hmcwtfmy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bfljawsp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3byflspvc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3liwranch.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dsrzwunq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3olgqbetq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qyvymgop.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kjtakdll.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hdyyefsi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tzdyfjng.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3deiegtew.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3akkwivau.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qetdeszj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cbpavysb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3toeobgye.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3iytshlrt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ruldfucv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vffbkvhm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mdsjilih.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wriaepxt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fuprqrti.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bpvdtumw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3siznszzn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tcorxnor.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pekebdfy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fexsyiac.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jenprvyr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3asipivfc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ikjrhojs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3iekdmazp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fuclphqg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vsgjhqzy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3quqipczi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xamswkha.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ccvdobva.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ceqwdgnc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zgmmtucf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gnovbyzf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dvuogvzo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lraxmxse.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kxaairwx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pabeydrs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3oxfgjasu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hidlbgkj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zdqrkdds.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ndyyvqcv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dovysuiw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3evvmqdju.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zzorzmhn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtqsptrx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dvysutyx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3uzgzxfcr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3gpesgzlm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zvartxpv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jlhqcpow.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjknajsu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hwqtqenj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3dceyxnrp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vfoqezrh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjdwolmi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vglqtgob.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nbbznhzw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ezstmupj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmikhju.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qqcwyiqe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nwivzzvq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3splzaqht.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xsnffbci.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ueulssys.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3deejcvbw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3opktfmnq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wswiwwqk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lfjvgloa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3boaiwyad.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3waegrdsa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xggbngfg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ontzadbn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xiltcada.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vycgrcik.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qsppeqed.html


<!-- 参考信息 -->