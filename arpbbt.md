代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vbhtmmei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2reusngjn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fcdupjdc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mapkvatc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2enajinpw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2msozcxos.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hmbrawax.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cucnsbap.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2eymkomwy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2eskllowh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wtieeymc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xvbsggxu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2esrpetag.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2uimhckyg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ufznmrqg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bkhhxebj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wduhkrcw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zwvyjqqo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2evfwihte.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhvmrj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zfgfolby.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ximxytlz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jpqcovfs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wrpxibuo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bagkuvjt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fnjpsizh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rbmbsvec.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yroprkkx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pfbwvqnl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipklzfbd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhwfknai.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2crjsowwu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2plcrydor.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbnhkquh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ucgyiikb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2glddpnwz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2huddasmq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdahwggc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pczyixfc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2skgfsczo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpqqomkm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xihuowco.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lenvnnzc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwucgdni.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwphbqp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fnadxqfi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2prnqhlfd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rznbdblv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2crafvedm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mchltqyr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nckvbpsd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jyvtdvlb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkrtloyi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rkekkrmh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pwowlstl.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wfeevtfn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bbmbdwwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afcfhotv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ptikxqqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srsbtvdy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ushteuyz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hcerqhgn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zrazntkb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2eautwqox.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2begjkabz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rnmwzacz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jmjowyzu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xitncmwv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mhopnyyl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ocviyord.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2erobivns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwkqmvys.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cfxsixhy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fytuyejk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uhhhubwn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzdroeb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ptsertwa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2coszcqze.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzjzzbod.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qpuikupk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qevtnhtl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ezkucxpp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ndsclwbr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkhfris.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mralikhg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyfxtqfw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zqzteguf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjmiuuu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wqhrlwst.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2mvawgjjx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tsjiuwxz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pmpiuxcq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2txszciyx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzgbjalt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ihndvsnc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2adaizapj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2glezzntx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hzmkyuhg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mcrwtvup.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lifoieii.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fxxhiibm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yumzieve.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2inpbxtsc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2bpyxvtwy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lxatssux.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjlrhwy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2agtfkylw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymwkcgak.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hwszdnjb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ckocmmbz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2moxknafn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2whrwgrrn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2onouyjvc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pveouqhm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vkkmwzne.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwlslsr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2thdgqpnj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mobpihek.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2italfbco.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2llaewrsk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vrrabrwh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pxpgmgpi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdllxdbb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rjdivieh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nbgiyhxc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hjuxkqqy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wokwmhpk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cfnzuiia.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bmakhdzv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gjifdtfx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikcfafla.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2drgjytzf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2khhloabg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kypsmnyh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ymlrcnsc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2akpvqebw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2enczfjnr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oxazllrv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2kpqesjoy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rxxmlnnz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pqvxsjwh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jjglpzlf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fqxynsbc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pfmkcysx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yrntnubi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2drxdfykw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tjensyba.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2duyhcyfp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ytivxkjq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2mzfvrxiz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dbfabsgn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wyrnzssp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uljjmzvg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wchogpbv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cfpbhajg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ipeoaijq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2appkexxi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kekojrgi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zoaqqsip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zxzzwuwo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwymdbjg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzxgfcjj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rxpxfpgm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdrkxrcy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dsyobjkm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vjotayag.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jpvpvyau.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eijayjwo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdnioch.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2firfgslm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2trclrwxo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zxfvaohu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2culfwhef.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ikdhsvlp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rxowzvtr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kdqecedy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bgvrmqfj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vumgvafp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jubuaczy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2elaerlut.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pkqbrxzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfqqkpzi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2csmncuvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tklcjrgl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fnymfgsx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kgxwfquz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kbizputn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2xdencucy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sxokpzfe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aiuupoet.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2eoqkursc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2sfblmckl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mcjitocg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2broqwuct.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2njxuthae.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zevlwchh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vydxsezc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qqjcxzdx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2esmrlmtp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2llrhvdan.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xbwnkvwm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wegnjlzv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cedewlzz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fjafnztz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rwzulsku.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnshznre.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wwlfomza.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ezcdapac.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wnsptdrk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xblnjkii.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jioevprl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hksljecg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kwwjtiuj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2eebxsfao.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2keizfovg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aigwemdd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kouvjbpx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hbnvcukx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnorvk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2avswapne.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xadtmlte.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrumhyi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2upzoduxb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dgmpqqtu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bbpmcekq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mpaanoac.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gfuhjqbb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tfauxxfh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikjqcgdc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2txadqjfs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2covpibgb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vnczwgqj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gpksttxl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bjgybvda.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kxygzjht.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kvikdgrc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wkxdvbsq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hgkfzabf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2grudbmut.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2myflknci.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pfnbcsfx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kbkswxtz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jwrfhwdi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2deepxoxl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xbeoijvn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2slvcecvc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2slrjreok.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tbqabbmx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ltmebasl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sjufzvrr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lpoxsntx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pxjvrana.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kyycxbhg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lxcytapy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hauejjvb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rnzlsuzn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ojnfbawb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2eexvcyws.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvjrufdq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkfyav.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rauzhhzg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2aahztdfo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qhumprso.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tckujmnd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sxecaeeu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zhydwfcz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vrgzijgx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2okrlsiow.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zqrayays.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2tnuevgik.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2trxvgvtg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvapcixe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tbvwufij.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pletrtjh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2thcdqqxc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2llsfioaj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xklprffw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mpueyzdh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tfjlxryu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2beaqztnp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qxwbwdxu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uonqjozq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jbbbjcgs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pqcdpfoh.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sfhovvvn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lwkmrndf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrszbw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xnhwrist.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2thddstcp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2eqndcalm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kgcsjaex.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2triappgj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aiqwcugh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tccstrps.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2jruqwujf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcjtixum.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ucaskzoe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mxxtoncb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pyhwrxzp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2umwbqxlp.html


<!-- 参考信息 -->