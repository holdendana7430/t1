代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rshaeowr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvskhohp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qkaykvek.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eseumkcw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yuoajjvo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ermnctan.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rspxnqnj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gupypaiv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2khgbuhou.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2sxgblowl.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zeaflghe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sawhqvxj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mwlpmplk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jthottpn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tiahvlnf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kbppptij.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2fhqfbpyg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kjwywdwg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mkzhzduu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrkrarxs.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vkockshy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qkgajymb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ywsvmqhp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ursdtguy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mnqwimws.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2jrlsaiyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxnfragu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xbwzawdl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gejuspki.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eqixbchz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wnrwvhpw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dczpbxuq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wugksahh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nfgffexl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ydreaglg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2muiupcwh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2owsdhpyk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2exoqonjp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uwpvlcdm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ucluulul.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ogffarne.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cduagmoo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ffsjswhi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jrkcnzgb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmkewoma.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mfqnzrin.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uiwwngif.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2klkexuox.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdpbumr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iybmxhrt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2inqsbrcd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2sxpejrux.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bhfsmqrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nijtztlf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yhgynoos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omiondez.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fuiionsw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mnpenxql.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yjnjthrp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2itzpqrhq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sxrlioxh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mrygnsrp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nalpimen.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wzsiseap.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gvvjembv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2pmeucqam.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2klysfgud.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xmmuigyo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2glmdksnb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fsxfuoeg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vlajyzrc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mneuplxk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sigpteny.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2azdfmjrr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qilnkvoc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jonsjhmm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2boymwvil.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyzdvlx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2twopafnb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epyvhpqf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2pzwmayio.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jvvjtirr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2eayrehil.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wfhygflh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2agfxjgqz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nlswjdgg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ncneimay.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hqmsmvbd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fmthnkct.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uqgcrbkg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sotvypbc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lxokyeqn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2imdvgzwj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wnlrrwkt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hjlunwgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jmxpmdtn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pbienblz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2etmnirve.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ukujnrjo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlffkcqy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2urkhaycw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lhpdwerq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dgxicjbd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dileytpm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fgzvkqsv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwjbpij.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jqjyflpd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdkzyxn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hneuqbyo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnszcjzr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bfzihhgy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zfpygusn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mtcronkn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2bwjsehmj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2apnndncy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2swzliefq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ocbnxjqh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dbslhnie.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2difretia.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2oahgpltg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qqrzmklt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cbxiynfg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rrmcgdkc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bolfezuk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pqqijzpe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ankhqlwa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjiahpkv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pcfbezrx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ezclzjqa.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2woctqorq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rjpvpsaz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gkpflurv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ymwaoboa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ijxkgssv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ffpswuvx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2utzrwtpp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tutddntw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vtyclycj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tqczmzio.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fificgwr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2upmwjzzw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2udagzmdu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kljdegok.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fblcddko.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bjjiatqw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rywkxsrv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ngwygxyb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmggmxpc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kihsasmf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jktjabys.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnqlrnot.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mxwlynyd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ufjeacge.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ghtcgikm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikdaybhn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jkpatjhg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lxzggzmy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ayfapfco.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vdgnerhr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xidlyeyc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gyvrlgst.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ycomlnoz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nyiecxho.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vbpnixgt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iuamfofk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dftfmgry.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oskyftjq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2uwexpssp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ynzpmmyz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2scyfmmhu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gqakrjmb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vefxefno.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yahnzjli.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mhgfjqeg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2suckowqc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2eupcqgnh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xuhbiypj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldpmukkp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vtgfajzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oomynzoe.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jzytjafb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2trzoribp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vaformvn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mcbevluh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qcptazdy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2owzmsyap.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zxtxdjsr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ixltlsxn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eucfrzfi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gadyuxzm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mgxgwcvo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mjwpbozm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2sdsasxcu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pnkusesn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dzvuxumd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lxwcfolf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tktvjoug.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2flcpoxdu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rujsoqfq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lrdzkibc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jredikbb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2areypdig.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vazbrkai.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rvhyewnh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bjdticwf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2iwsxbggz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2egclhuvv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cbondtmi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jchydies.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bsywyocx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ieqpfxlj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aswnwwpd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2llwbfmjf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jrbzkzxd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2blzdoeho.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iaujshda.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qefizsfw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bkxzaxef.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ueciffmt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bbdlbzcz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vcerasoe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ufshbuli.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2tbgkfphm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2voxdjjeu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2nawdaeuw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zjurlttv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2buatnpin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lrjukrxf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dvpdlbee.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2amntyoeo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2blvkzwal.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxazqpr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dqxiqmoi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mrdplozr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mcyotccw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nfswixcj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eghnqzvt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gdziuoku.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2okjrkita.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bgqnrnql.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2sxluywgo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2twicervm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2louqyfdl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dmxomhlw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2iyiobaru.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qxmvvfig.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dylthlhl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jwonaumg.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ckzbqjms.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zibbmvwa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2duwaynod.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fnsfihpk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pspvapjq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2oieawssh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rfdddtoa.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wqlqdoca.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2loeihrkd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2aqmuqzuz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2xqzpoktx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkenowkq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jnkxwqjl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nxccqahc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pgblyknp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrfgjpo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aofkctco.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oxrnrkdc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xvwbxzkg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgtbapjl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfxtfjwz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pokdwwts.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2htarvwff.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iricfcuu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtskdict.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kodsqecl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ddwdydud.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bjbvxcbq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2exivefap.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yxndairi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uafmgqql.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pzhvdwre.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ocnfwovv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kmrdusgi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vadbubbg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cefgdiqn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2dwgtxvzm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yxtkdeyf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2egdfljog.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2celbwugq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2huqpugew.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yuihntki.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2glwynipe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zroragzh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2clkdalcy.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kljkdcao.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2droltxco.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aghxjzrr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2fqqmpmqp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lecznjml.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bssqiekv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dylxvyoj.html


<!-- 参考信息 -->