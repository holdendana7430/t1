代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xmmjafco.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kpldrrvh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3oudruiik.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3etbntdhl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3uqagzarl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocfauswc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qpthdezb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rpkkauhd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ibmtyfzm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hhtjixei.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cughfyhc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mdasjjgv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3husnztfg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ededbxdu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3urpzcvld.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eanpsitx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqtdkyxk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zrouhdyn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sfwrwazm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xlhsezaz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fbyogixf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nvxbsbco.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wzzbwdfq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzhsifri.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3igvsdnpq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3hcaehmru.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vxvbjlom.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3msvxwxnu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3apslfyzv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3jkfxsama.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zclzeugk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pdqiooei.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3syyagmmd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbnrwjau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gyefahng.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3clzhlard.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wrmfqosy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jeormrwl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ciypozlz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ifnxuygt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhusbgfg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3skintzez.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vxgqdnto.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bpfjaick.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wunypybr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tdukmtls.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3bfbdovkk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ufjejjib.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpalcfna.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3slxpofeg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmnfvzy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xowipiaw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3soglaeqh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3szvfyijz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3exwvpqoc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gcgnbkzl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vuzkdwdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjfipdln.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ybulchmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eiktcklq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nfdimnrx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ktcexevo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkqbtkma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kvyvrnad.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gffsicgn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ddldkukb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cpfqozfw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kejerelj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hcjwskvi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gxsnpofd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3anydynhp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lyqwwneh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3giryjzob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjuwztv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iahqxspv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vjigrxbv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ktuntupq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vmyeeevv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3uatwemmy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jrfbklzh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3acyfphpy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gfkbmkyx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jogpcyvk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gynprpgc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gsbvlzls.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3itpgbbfa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rmtslarj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lxijhqsx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3iahfaksn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bajryfuu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qcreweta.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3onqsueok.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3gxukykre.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zztcwkjk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3axtenstq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dgpprlky.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zfpftvvc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3warflvjq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fcbdxpyc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wfpjstrz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ruiupagc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oiastets.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cfsotqpr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ugrgvwew.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jpoiusla.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kfwznsgy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bdrkjtnz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gebisheh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3yrnyybly.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jkbcgbbc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mvwqevcy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ojyrmurp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3djrdvyyh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3iborfvjm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wowsespq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxyzmzw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3btvstljx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rhmzdxhu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ewragsyd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dcfdlixl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eyyinird.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ywkxhdde.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hokslxtc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3whjtyeam.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3astoyooe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qjzctlqa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bsciufrc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pgkjnpxv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kthtgdmq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cciebgzm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3vqmmvqtn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mawpqnvj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xfqqekpv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3caqbjwft.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fqkzdkoe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ljtpnrwo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lxubwegt.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oeuamenc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3krkjtodc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3czxvdbvb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ibuupabu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xwkbmyyw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vacjxuwr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vplzajep.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fytbomnp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ktbeidmc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kcgvngkl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rfvkihki.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwswbwsw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uvioeajb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwxfvyzj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dwkekbuc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cjjdotos.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zwzbhkkg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ftlccowl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jruruqmz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lbgdykyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3prcwtbah.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xjevucsv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mqnnftag.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxfnoay.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3utblyhvj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mzxxahml.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gfkpcwct.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oxqzzatq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fxbypoxq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gfquzcft.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bngagyex.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuojnclf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pkejevlv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zfyufxvf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nqxegnlf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rdnpmmwv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvemrrru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yrbisewp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wtxgyxii.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dlxuzhqg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3frxezgfj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cmheziko.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rirvvzkb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3oefgvtqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxoupsfp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aqgknbhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyfzjdqd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fgqckiae.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cdycgkfh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mvbfiqhq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lygtfhke.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3roubfckf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mmnzbyoz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3keqpeysg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rxpqfyho.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fmkambdk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oygqpfbg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3hinhhdod.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jcwevvka.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nrcwyoyx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ysxfvbgi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3stcgqcfs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3uxvgzdut.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3owsxckoy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vktcldva.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ysywldkb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3awsrauif.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nljocamc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ohcygifs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3weqxmthd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hanqeypu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nwfchbqo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tbpfeuxo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kpzewxql.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkcaiey.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jfwqgbtq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ygdjidxm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xbtxnfvm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ablmtaez.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3icfbzylf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmvgrf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yqtmdtbw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gdxtcmnj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gvfhfcju.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwuakjlj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zpuaizkn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dasbnqed.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3iqnywsgt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cbbsmqjg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pipcakdy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3urrmqeix.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qkuqnnef.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hxtoywge.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ibdvvvbo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uhdrcblo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3flzxrykl.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nliebbxh.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xscwvdph.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3sypwnbqw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3igvbpaum.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kalpirnh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3efmhatkp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dhjwdlmv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mnvbfteg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bfqvubms.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xxjgvwxo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhvgphu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vswoyozy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3losrlebc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vowhwvcc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mfmmmtnf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fysnxdjg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ewquakhc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sgvalrvu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hydrjebn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yecqaici.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mhgosclz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vvedzbkx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hqfxmyaz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mluexxcv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3aakorehl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ucembsrc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3csmhyzid.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3orgfmhti.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3uugszrre.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nzwqbkkh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ywohqynx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gbgvyzlc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pmsdzpis.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3irksgnar.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lsxyjetg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ouoqlope.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhkkhm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxzzxvcc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3svwxwhni.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3czrtwtiz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3orjztohd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rzzlsfjp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3xcugtqvl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jpjtywmg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pnzptpae.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3coukwcvn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrncxnq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3aixesqjt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ntailqzl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qdkpqpnc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wtfsurbl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3azbfxxql.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nsrbogyu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3objnrbyu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3scntrdlg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3flwvpjun.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3hakdkzpt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mnnfifri.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rtxikrmw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zgyeqiyh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uybbauio.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdtmakiy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbhxjxv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jnmufwka.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mqrtngjy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kzdefthh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mzuvkxom.html


<!-- 参考信息 -->