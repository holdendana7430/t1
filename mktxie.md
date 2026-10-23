代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3aebapwzq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eefwoiwd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tonyfvnc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3peohtusk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jrxrizcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mbddkplz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sxymontt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gtehslwp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3asghzywi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hzhdaxba.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ggaqeilq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fbrvkwhs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mycmfmpb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zazqhbom.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yijopydj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjgsukn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqskflni.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yrywqsig.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnqrzdhh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ngjlbfbb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fytfkbdk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cqdojstl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3umazfrxc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidbypfu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3aliftkia.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hgzxzext.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jbaaucov.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hrhxiexe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jatbtdlf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vpgwftet.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdtqwpmr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3casinaod.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gbkcvyef.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwdshnaq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gwiqxwdu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oaxjmdvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lvuylfgp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dgfwxrwb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rqhtactq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3frejagzo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3slpdgkws.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cmjhnlaq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lkgaexsf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfqvkqtz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3adraioxl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qixtoosr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3shqaqgrm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3udctqsfx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khjjjkht.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qelnypgc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mrjtrnlo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yuexyvyd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yofpgnpn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yhrquvyq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bhtqsmnm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cjlgsgbq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wxabqgyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avetbfjj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jvaknicr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyyzjkkb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bvmuavqd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3alnutkih.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qliczuai.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ocewmenp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sukqpcha.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zdxkbejv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cwkllfck.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aspvutac.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yykmuouy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3diodqxhw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jtyvrkoi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uoifxhlx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hlvmrfih.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vndslcgr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nujmgnkd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3aimmwyep.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztaezzvn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yyntvwyv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3iczqepre.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tkqibsnk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3quyvsdtx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3svelshgr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3siwtpexd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3beuawocl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uthhxqqe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyobscoq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xzrnxtmv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3llqpeelr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wjikmuhp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfbtazb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3udemedbb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jfelykka.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3gmeyzppy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bwcylilg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nmrxzrtb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ljcouvnr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pjxczioz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqesevdo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hdkhmdro.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dewmoqte.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hrhznsta.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3clxkqczo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ujjdahgd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hyewauns.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbrbfokx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hhtvyjut.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cokmsxau.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmqpbjn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xirlrouw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jvwnclwy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mzqifrsh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3clxjafwp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vsqvrybf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bifsqkyi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mzbwoxpo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vhwgnmuc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vqilejji.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvfdrxq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vusgnexk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xxufayln.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3szccyasr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lsoqlrcb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3twmubgot.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3isdbqfuk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wjrwjcmq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nhjesrne.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yerlvksr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yquiarps.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3fqdhlzaz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cbftodst.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3otiraevz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ireksexo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ioletela.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gazrmbtw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjhhskeu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jjthfgpe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oioqonan.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yprliorr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cksfwjhi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xyhyzzgs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3efuiyyvv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mcvaqakh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qqvrkiii.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qyvbfjkr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3szjdooti.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zjcpqdsr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3derpdzhr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blgokjyv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjhxhyds.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjsdgdvc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjczeazs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsyqquov.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dmaqznvv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oyzoxehs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3psbqopme.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ciwmrufr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gfyhtcxe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3erniphog.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uchirngy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3tuvhoqwv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfjonmx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3srktbhbo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lfihicca.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yurqiqhf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3epmhkogq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3diglmyra.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kahyiswc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mbkriilb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrjrnzg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ebasenuu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bkejrjlx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3klosrdgo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cewwbrhn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jxetrbkn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jjglfahf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3canoirlz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oeyvelnt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gnwkchjt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3djomrnan.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3impzzxtw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nzxhymwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guvvpink.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eashusha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzaksldp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3sozgxjuw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nidrrczp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uzsdpnnc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hlymflkz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tmcalteb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3habrswdv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vroosbkf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gmzrlosx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qlhjxuxp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rubpipgk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eihwlbsm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hbqiurja.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ondmpxry.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jcenykrb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ofyfaqdy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vejazgkm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nxdmoqfe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjrxqlg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tzuxopuw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3zjlhgnra.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dceltywo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rcqenzqo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fvdjjvhx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mnqsijel.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qmvtttqk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vwhgutca.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fiypizzq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3afidqven.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3vexkhlci.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3flclapbw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gnfxgjbu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zaczgjbq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hiqdsbmf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mfuxqizb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xtmlqtso.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tmlyhmkx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iobbzqjk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fyrplqkw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3domrtfpc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3onjfuubz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tasixntq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xnkfpilo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ftrtapqv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hjuavfkt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3darjpznk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xvlbiwga.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3widkgrby.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3akecufir.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bnkjsnef.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lwsqnusc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3umxrafxi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3agiirejt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hhmrivve.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zrvoeqbz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vktjkicj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jygmqfec.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3yetodcjx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gcziysvz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sipgjvbf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pzvjjstp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3znnhewvf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3swqpatfy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtycsmly.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vjzpmjdq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wvqtwbft.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kqnitbqm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ihnqwlpv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gwomofal.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dmdwxcsd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lkomlqyw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ksfvvzoa.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fskgxkuu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3antfpval.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ugieusxy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xmlmxoml.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gqakjkty.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ffacauyb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3prvlwlts.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jpyfqywd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzczhqhj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3sjkrcpqa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nivfbkby.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mnpclitq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fwzswxvu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jhfstygh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hcwfkulm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tafibyed.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqzprgvk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3egptrtwe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3goebixvr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3sbsvdvov.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3njqbwjil.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhuchiuz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nkefztrk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fwodhelv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcddaiu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rptufkxd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ksaqydug.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bykyvsxo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnqprpvh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ppdjvgks.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kkwtqrgn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pldgbawb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ouczyztp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bzltsnwc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pzljnwsy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mhngqshy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pzbhyurv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3slbbqxmo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ktejphog.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ghaiehne.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzawgdzz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gtexmwru.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jirdiuse.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hfmqgjtu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zvqpwteu.html


<!-- 参考信息 -->