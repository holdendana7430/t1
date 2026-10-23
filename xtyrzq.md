代发 wailian999

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3cipuafce.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lmgccjeo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3doioquvb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ffgafqnq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3baomupos.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ynvbwqxg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ojhdmgel.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxqbuhxd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sdmaeezj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtumsdyr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bwsgkowo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jodoccwd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cuiazrnh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3agvwypli.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3sbhoqznz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3luudnycj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxuoniyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3eaqvhzxx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zdffcacz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nrlvwpjx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ssiauect.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gfzpwofb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3intrpqck.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dllbbhqe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oximtnyr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tyqgtnfc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3hgwgwoya.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wijdpsey.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zfdyxnqp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrivnndv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnwihbia.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xxixhdew.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkazhgv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hxmohtku.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sigkqfra.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fpexkfbp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qlwofudf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bqbosuvn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3brmgikkm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bswjlxps.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3juirsryt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tzdaqzpg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pjuyqqen.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3elmsksun.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jwosczjf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cvbedivz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gnjzmfyu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kuieasyy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yvpsjcck.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbbwsjxn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lpwhsjxy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pedfewzf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qwpzvjdh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zjigfxfj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3beslbptb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gxuyzyqi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pzztjara.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qavpecyx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ykkeljiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymwmojok.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3spsprswi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3houvuyrv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sjkrbmaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nopeumua.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3reeuaiev.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cwelmrzf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rukywrcn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3txrpueeh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pvtauizz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yazzjcek.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zwcufbjm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmfywyfl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mmocinjl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ajngnrps.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hozfepru.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jdstsxcr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqfexnee.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3klsviokx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kcsriins.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qamtwmlq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nybgqhgz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3unovshwg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qhjpovnk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3abcdqgcq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iihxqhdd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fvbbaiby.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yugneujx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jtproqby.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fgjyjigc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3iovuaazo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lprkjocu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mnfvqkzo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3eivpcvtp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fothkbbe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3edfwfnwr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vwwfjlsj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ghyvvaqr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3swldltvf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fktttjhc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3egxrowei.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wchvotss.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ucnlirrp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hmrffwag.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3tqaevgcf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yelqemdp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hkyzzvht.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zsnhtwsp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cplsoftm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ezdzwsvr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zkshsvyk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wnaoegdi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjjoqa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfnuusez.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sfhvkcjc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xpnzjule.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xahtsulj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oztxtoql.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jrjrpuqi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cbkecqrv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vubifnzz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qwclcrbn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3orymqywp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwpfguqf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kiilzmlq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ynuhcvof.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3orxulkus.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3crycxgsm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sxgrname.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ttvqscsx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mudvvhvs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zepwhcdj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ozmogtwf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pvfpdpic.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zzjpeggz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3clgtydoa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qlaggrwt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ynbnugil.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nthzyhle.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kiywtnyk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yxizsxdz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvrefaxh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rsdtidhg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3renncdxq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fodevpnt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3npmgsvhe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jspzlcns.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ykzguukm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wdmjcgxt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjcpzhpx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvlnyegd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3snvsfgwp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jukqtzkg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ibyypieu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kywebecj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qzuvsyuh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jfbsjyyr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohdtamdy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3srspyhey.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tiablcxy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3owfvmook.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3efwzdgcj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bwubqjjq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sacwvryl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cgbeyvdg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdohklqm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bazuslkd.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fuuayvrf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tlofjdaa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3chgskirk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dwanahbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyestng.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tpgysmjl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jzetetac.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qzsdsyxy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcaftsf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ihnzclqf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lpdvejez.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3stovttvy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxzkplj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fahxkjbh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3anjwbewl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhxjkxvz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ljyivlak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsimvqck.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vefqjxto.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ntswljns.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fkfnkfgy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3trkaekcv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3upogdgra.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ciecktqo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dqzqtcqd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3evnotczh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fsxwxxsw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ueznyzxi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tmqatdiv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lwdckcgb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tylfwjmt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pxrbhrgx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3babcduwz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3szjokzii.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3yydqoyfv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxtqvve.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zhvvckig.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tetnsptg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3njrpytrt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsiukaak.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3gqxkxoqg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3znzlsoht.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dgsmueik.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3scyltcvs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3twkggrlu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xpbzhtgv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dpmgzjkm.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jnfoqahe.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rgigobfc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3udoyfotk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3evklkxnp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jdmluayk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bchpxfjk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cvdxykfn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3niaetdgw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3msgdalow.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzvprb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qzbohnvo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cocldveh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yusgydpx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ciyxlggu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fcyadsel.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mzugrbad.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qqzuawrn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fjdgqcjc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tabapqcv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hktnyjjk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vbckbtgk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dfkfyxtt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ihouualw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uydbqomb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nolqozzp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xxkthaka.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3iregysmc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jznzgrrv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3upoxvzzz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3sxkoeozf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ssypkesr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zzezedmg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sjhviskl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3akrdoycy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gqwpvdgj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pwyjtgfz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3yqazzmvf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dbsbvnmt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wmklixuc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3rafmlnhs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3mievrwxl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fuskelpv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3iapqutkl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wgamnbqd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cyjkmegb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zmgaoktz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iatkmsns.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dymmlujl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jvemzcap.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3izjngvvq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ycobicak.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3iztwokuc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3dspnkrlt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zifptcib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dcuylree.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3issplpny.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3iimbwkvv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jnxwunjr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ehptgtgo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bdxcyncc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmowdde.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfaikknm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oajbzegy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pevsacll.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3afqyxyoh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rnezsorg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bulzlcph.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fmcygrrd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rmsmkdqp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fgddhhpz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hsqhddxl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lqizpqfx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dvdrixgt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rtbdfzmm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dzvljcpy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3adcptajb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qfomanuz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gmkezexy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3evewyehy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qleigmya.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mlleypiv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3heflghsi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qeuimxrz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3otiwfkwl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lrdgapny.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xhgjcfou.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sxwhafdx.html


<!-- 参考信息 -->