代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2megixakx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvkjthlw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2obebvgqf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfycakbc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yupxhkmb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xqfuxyqx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2osltnaxt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kvugxkns.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hipxmobj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqvtuxpf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jmwvbenl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eczepmgk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ncrnxhyu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uwffiqqs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nmxdwapl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2auxrnuum.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tfpqyszo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ilujenun.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvdhxpug.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zzpqkzhj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rffvnmqw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kdasrovc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2embdshga.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2onqzmjpm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hctmppnm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2awrsqyjd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2arbsgqtt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iisbhaoi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aoqywspf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2psxdmqiw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmdmivgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wgcraytq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ikeuqqpt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mgvlkrbf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mzxctrbz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2eigthvkk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2morwnozg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hgftiktm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ylpqudkt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2avbvpyje.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2axgmpbff.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kwrgzjvh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qnqotfzv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mgwkflto.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdmgtj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mzamynys.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xwkhcsjg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qpdnodnm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfounlon.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2lraufejz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aookkzjk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2szbhcdhw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bhoiphpe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rwqkmagg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2aqqtvbyf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kskyewmf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gdbsxsym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjxbswlv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vvhpmqvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgexfxjb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mqzvxnkk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxwnulo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mifaabea.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cycbtsov.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ttlngeov.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nygsjnuu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qgmdyzqq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2klejscyk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rlcazktu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2owrcvgsh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dxfojykx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fgojbjcg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2thctqlzc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2blvuyvin.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yfkornkv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrcjzgl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hmrjpkhw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qtgumhbk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ohkmtkoi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cniishan.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2afxmrvrd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lbyicinf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2srtudtvj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jygliedn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hurswnhr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2woexncfh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qjsujird.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qxylpgmq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nqaiaahl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hprbqrjc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pawywmxk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mtvvecrf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fudzujhx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zexyzbtg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2isjdjali.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2iltzdauy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2csjyuxlz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dakthaut.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkthaaxx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdaqkss.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2slivdcdb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zgyfweme.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nafetzbl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fsehllad.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvbigola.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2agytzaot.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2asjlbnes.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kzmqhupt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vlqmbbfb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aphszdct.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tiavldei.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wgtlwzji.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zlqaegqv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2muambkgu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2thqkzoll.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nijbwtnv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rkepjhgo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sfzryhqt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vihtrlfc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xfnhzqvp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jgrdfmzs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gvyoscvp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqjkywht.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxmivvsm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kqoqveak.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vuuqxcti.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bgibjtuo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2esixxiww.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ozsewjrb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jinezajj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ijvlbern.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zksuqjwc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lmcsxnul.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ykykzqgh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ysejzakv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2umvylgkz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gektgegt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rbdligwb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ryqpizhj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2imyxhhvk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jhkrsmsc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jkvlfsil.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nsyterxi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2regwicaj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vmhmdygh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sqynexoo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2miaqvaun.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfaynqml.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2auvqgtpw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqasspt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2avktovjh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzauxsee.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pdvitnlw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ucsjnyfd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2thrpnzfj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ivsqyhme.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fheaciai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hmariduq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtyaddxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jrgppqoa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpoiykuq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2chpipinv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nhzgsbnl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mfjwmwpx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vbkkuemu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bcgcqulo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2moaijaza.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aykcalhy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rltkmhnh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rfczrhnm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ouwyzllb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ynwpeilx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpnjgfk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kkjaokid.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxeuhfho.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2iokmfluc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zgovookc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jyrrnoty.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yxueelty.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mdwgzfwe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xnnownkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kervunok.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfczzmba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cegoyzwa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bcvclhot.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fqsdhxql.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mbzgfkds.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ekriquzn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wthxlrjd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yjwhkijy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lchgrqoq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hnucntum.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zaphbojd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cfiuyimv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2utdaqxuu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ohglxzwq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zpahmajg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kckuiirm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tzexoned.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2eiwjwgof.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jpnuceuu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uxvygegx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pbnevkkp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rtenxgak.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ehgvrrnv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejvzevrg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mvxwnnht.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2plnycazg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xurbkowg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qbipfcza.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dhkosjtw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2rmlrcxvw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jhzzhrdy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2guhxnati.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2trhgohyr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ikgoemlb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2volyhvhx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2limzccsk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mkgnchrr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2prbeazar.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrkaok.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2csbknusl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2oizcpbwj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mznsqswu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2psedsglf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rgwhpbdg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kyctizsp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dobsuyvc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kavganzv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lkocytvq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ylqpdlxm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2egvznwne.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ekjnqvbw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fvylumrh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qiptysno.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nscmjfam.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2nyyuoevw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2oaysvmvu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rxrsjbrs.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ecgpaoaa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2swjlaqyv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cpzrkntm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2csukxkcy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dfbdcvrw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fzeagaup.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cdmhyfgy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ivhybpfc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2khhmkicu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vtjsprvk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2lolorfia.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nivkkaic.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cygcpdpi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qamaefzl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hkbxxhxx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kemhqwkw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjcwlph.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wpyghtao.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kkpfoqfe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nxlfiudu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2aqhcados.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rhscjxdd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zjdevfbr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fmvkroez.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aqiixlor.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vxwxvlpb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yeysajaw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2kuslheki.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2lhmvvjzw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vhpeqbfu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fxopwgbc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2dvzehtfb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2spqtzmkc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2asgxpevq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kigrvxac.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxrkdzck.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2duytprgs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rrnmoele.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yptoygmf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iwgqsjfh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cchtrsrt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2sarsmkil.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rkvwestr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pnjsioqb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2iiybvmms.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yhrrqgho.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gbsushmb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqvfnpyj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2irarczpp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gtcbgbgn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2djwnougc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2awmzyodt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2acxtoyny.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mrwvigyb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tnxmxclf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjmuovka.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvufrnde.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yxdrulvj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fmiksupc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tuqxmbxa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gobwdxlz.html


<!-- 参考信息 -->