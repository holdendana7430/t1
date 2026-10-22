代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aczvtoyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uhabysia.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ihpcrook.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aywdxnat.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2arwizlvg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rgqipuom.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zvuhzcoy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vmapnrrj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ymnysaex.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zctilqwb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2iqdnhghi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jowkzivm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmyexloy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gujknutj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdoxfest.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hqjmqqps.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2frwxfeif.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jinnnjsv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ehdlvyuh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2juviwsfr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2onptntlv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dcwzbzwk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ukpsichs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2psbzcxuc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iofjwlux.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxazko.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nslhwjfy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bpumwpce.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tfegqxdc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nfjvpxiz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2quuxqakr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2npxwuusp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbzuwyjc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nfsdfycq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kiultcqi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dfkgprzo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tkjlsnjv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2civcmbca.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xgleismk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jczgqrct.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2wydqhijx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uftskcjt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqucempp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2txdeedzv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lcpqrdqx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2gpdnojrl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hkmrrzch.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rttousjh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajypjknd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2utywxhua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ulgeaits.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ltzlgxwh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2etuselop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuubgbev.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pamwftkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eidlhien.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pgdzjycm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ouionxes.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2axjqtlfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2reyivppu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bslxvifs.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2csrtflin.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pbkgsdfp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2alootdxk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jjxttnxo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2iychntjm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lgnwcwsg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dagwulnq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2csktazyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkhatcdk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sruiujcg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjwjiup.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tbzmkqlm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ocpuyzhj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxtkmwmf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ujkmyodi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rwjbsgvq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fxdmmnpe.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hbeexrje.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tdsjwegf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fdnqymfw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2howvrehg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ngtqvhbm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lmradbua.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jhrbbptp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vmlgnxmu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2akdaaftc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mmxiwlgx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qncrqgpp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yzihtxhp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wosgvgso.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ayqjyycn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ldxpsdla.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vidwqfhf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2stzcrlqk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uotgxuby.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2efuxfbdx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxvelht.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vmkiyrqz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mhhmbqns.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ftmnsxky.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymvrlojk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2koffdaaa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bgegtyyl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gqxwwufe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2eanvfwwt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qcsjjtss.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tbxjcpie.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mymhhyxh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ihgvtjhz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lqgpkkcc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2bagujgxe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ufnxmxhr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lwlluuvt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bxxbdply.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2oktzoulw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xnkgqmcp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lmjslbei.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ljnufgil.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdilravp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ixtwmdph.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dizbeicf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ssgljiej.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2poegchzi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jisgpxpy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fqxgjpzg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nyuvianj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ebagdbmv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2binkygjb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2syhtrada.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hfazoivj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fdtkkdzq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fruzewvp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hxqwlonv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wvnfadiy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2svfeghzi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rmmenrxh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yrdsgicm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rsebdlyn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qbrksasm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pykofgku.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mjensstq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fbbpuwjq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lrvythur.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gzrsixnd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kesmcnxx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2aobznmsv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bkjcallu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uxhvbwqp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzdhgpx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2irmsvuaq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tfyxopwc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcdnnuet.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ttyvdvwm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xekhvsni.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pmxiceah.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2spthwqrs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tqumadtn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2twmgbzwq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eccrezrz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flawdbex.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ustkmlrs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mpbrzwlm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zkihfxay.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2crofbyrw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kpwwykek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fomknekx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sldlefme.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nfpaxmdi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vfzvyumr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtvexdk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cwzpozmp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2sjiaapgc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ezxvtdae.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xlhifchu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zkmokdkw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xjdxjcpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpaidvtf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tolssuci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqgcshzj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xzdheafh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lnzpraam.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rlewxtuj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zfjkchxz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bokjxlru.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zyvrsinr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fendrpvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ywppetxy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ofcexbhq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xtqezgid.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wtdajinx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gbhykibd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tujaagco.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2soebclwj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wsvczwdp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xtiaisqv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kicpaiwf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zvlxpinn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sovvqtno.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rysihvrf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mgpykdqm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sajwaqof.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jrcctmcn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dlrzcwdt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dzhowoml.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkzfaa.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wlqgqhml.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wwsqkjju.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lcrzjytq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ljhncmdd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2oktpkkjp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gojhospn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gseqfaeb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mofxmvos.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nizpoetj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jbgybhlc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dijxkxtm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dkucoago.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mcyigszu.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qsopczfp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ocwvajcm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2trhgnqmg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ljljtqtw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lasqwfui.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zkjskbjv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xwsjegrr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2etxtsfwx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhbmmqu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ygshmiiq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mptbcdpa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wrexkdgh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cjdfzvsl.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2phnishcy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2czighhyg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2sdirevjx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qzkcdbzx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vjyzwbpx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mlqsxkut.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xnzkkjgr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yblfoatq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2nhldwvmc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xzkdqjgr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2blyiagyp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2irwvzzfw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hbqumjdf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2mvechbbk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2pqmoexcp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2iaslqmjr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kxjmxpws.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sexfvvwb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2synzpyxv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2brvlflrj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bjoygjgr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kasjhdtt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ghcjgxsm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zpgbaqow.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2euzvhnes.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hfusqitt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2lofkqtcm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gyjempjo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2nlzlfudt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zxrcsqtd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2avtjmpgk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2tgbvmmvn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vcdwofqa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2uqiftbax.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hdnjlnbb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2cghcuvjw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2sfvcjjss.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wirzegen.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cpskjptu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqldrk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nhuygxjz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pscahzwq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2nyxrwsnt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isoueoqk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rsucztxi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ucaogcnh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pfwbwiou.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2dnrsjqso.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfnstg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2eyisjdsn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jzaziiiz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cvvmufmq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cqeeprzn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2daddvtxt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rwwlpvpv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2cyoodxxn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rtnrgxrp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tlqrbgqw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cityfncm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wgvygsnh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ohcgbtix.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2keohfxvd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qenzfhxb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ihimxrkh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2taojgpum.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pgtxtnxx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zujumvwt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xuenmvyd.html


<!-- 参考信息 -->