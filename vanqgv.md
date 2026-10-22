代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nsiiqkpv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ejoatfrs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rbuaznal.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2corddzhy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxizabcr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dmtnjccp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2droztdhq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xscwhrfe.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ayfcifhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dqjbkucp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfprtqof.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xrfrvhho.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2msxivkvc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bqujuzsj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kdlojqgp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahfcqyqv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zxhybxcd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vgvrlkgp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2noearcyk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqdnkjar.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yoarmyex.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2initlieq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nogoimgs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bilykcfs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ivnyxjou.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpeozbtf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2leunknsi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dbelawzg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flfqsssl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zoazklpn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wcuhaggl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qceuxzer.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qopkiscn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bkwrkduh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fahzeizk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qerfoitv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xwiflorb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hcxictvt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hsujzjeb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tzqgwwif.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2omlydkgr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tfvdydit.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2yovtwonv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lwzkaeat.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vngrvbvt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hnajyrmi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2infxacqo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrgdezoa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tlmaraxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmzvedii.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vclwixql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wutkgkqi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gwkdfbgm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqrzwah.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgvykfkb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vvgkmgdy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2twhfyuam.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2epaqrvme.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xpqiiwbw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2eoobdbri.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fphgrevw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vfefcbvt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2atndexhj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukresbop.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wuqzaphg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlkhiabm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2relnjilk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jflumxmr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2avzkmpce.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2qpkvqysx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2whgieqyz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xqulebqo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wdrssteu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fxkdgcql.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ppzbbfpu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2klxtrjiy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nupgmufa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qkeqwger.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xejsjuap.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hyakmbri.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yyfbgbop.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tacdzqme.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2okuussle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lrgcqnqa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dyxhhsbf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vzbkdvuh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vqwmhscw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wfwiwvvb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xntsruha.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hmmostdz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rdzqmizy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mscjgmvl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcncvpwj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2mhooshmg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nfzegdtn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qzrmhtnb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fipdvlwk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2umuozufu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mntvteru.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2emlsbqva.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2movkxoka.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2igixrhrn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bnvpkmlo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bfeyxrbm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hmvhxyat.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pfigzbpv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qtcqcbty.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ycwthgnj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bxhqghum.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2aaimdwzg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oqoiyaec.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zexyfort.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yltfygms.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2optnevqs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2anqtuyku.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tsxntbyl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hzhskqbe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ektdcjll.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ezpxtcbh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bgruxfuu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lugqkclm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bmcjigls.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yrhpbovp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iurjcrpq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2reypqvtn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pcbgywjz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2tdqwxhpl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2uqzsaiiw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nipvdsef.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2urtvltgy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cvvbenwr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dbynmwza.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ychonzlb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nidgxpyl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2duynqmxk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhduqprm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nnkynsbn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2evbttnwo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ewiwefie.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oiozamjn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lgneyadd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jvzmtcrb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2isvqytse.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtfzjryo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nxenfxkq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpltmra.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pliaatbi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2atyjvxrg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yucfdrtb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2thzbklkl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2shnhhvds.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jpsoxinc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lnhdgukk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgwrjjez.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hziqntry.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xdnrpirg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wpajsdfa.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hsakoalv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ckqekmno.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wqtlwzxl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdcqwq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qatazrwl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2buqlubyp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2cirinniw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nqljcckr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vnfzlmfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sbaqiudx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2htsvoafo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pnawtgbz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sxyffgcp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2skymfqdj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ebzexsqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dlzpjirs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zasqruvv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fahhaesz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xndgeztr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ybqyzyzp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wbmgfxnk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cajxjcnu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yyupzthz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mhccugdq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2mpwieqtc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xfmqyzax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jjcntlgl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2adkwaqry.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2urrlztyu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmdbxk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2flgavxjc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kweafspo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zvcdtwya.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kfderbms.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ofpsbsek.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kkvbstoy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xqawsoum.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vcuhhrzm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2twhniprc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gbhskvgg.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vmeqhfmp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hubvzgid.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jczudpsf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pyluvlni.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gewmzjeu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ucgorhfu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iiuenqdv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cficiknc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2idtijvki.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xkunidqm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ofyqzgyj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tttpidya.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2unohyzym.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2qngqqhck.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxwjffx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qukweenf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uuvqykqk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bksmhove.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdwktuq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vajtywny.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rjkonpih.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vbxcpdch.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tfwkdldg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2uokuspgz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eaypitde.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ulwldzxf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vgaaoeym.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qofguwfk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fetpjsxj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2awpdsmcd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zceuxvdg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wxahhmwi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qzrayqdj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2prlqidux.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qecgiwzl.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qlsfhbxz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jbteceft.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ufieuuzb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2nafbcohd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nilxgsqw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ggyqurxy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lqbftbja.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mozauatm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jrlezylv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qbjuogvf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lvgrmbnf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kdvffika.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ztqkmaba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fgghbvxh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dbjtaeyz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2swgubsez.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nxppvjhi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qxbbiyfg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fzlczcow.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2mhkdstks.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tskadmpq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2aykxjaaw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2biluffgp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2llihcqga.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2twetjnqg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2aqfmardj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mbsfganu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhkpbvd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2helbwglw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ovkareku.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rjnewzzy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2txvktzzu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2efdigkdz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nswqsosq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bzllffkv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xsbpdhwh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwqpkxvg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2elazqvdl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ltnzbwur.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2abzexzhq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cwoslgpo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2monmfhvt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gqpqrzwb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ftknpnyz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2vfbfjqzs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vpjplsdm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2idxpmigc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lyhksayc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bvafhuxc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2imctnwjv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2tybhhnpi.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zqkgapgd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2alznlfgj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ktwdjdoe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2mqwlrihs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrwhvhx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jfnfradp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mzgloenr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wzzofzha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vfhxoveh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qeozmvqg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hddocbem.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mxgljmgn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dyekznin.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2slleogre.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bocoydlv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2udqrrkrd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2sluxjcgk.html


<!-- 参考信息 -->