代发 wailian999

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rvaamulr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gglmvmni.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vskluevg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3okkubsvz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ccreykol.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lxzjbfxt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cnjyogto.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ttxvxilr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jrozdrwv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hqojxmmb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ehojacld.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vszlcsuy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dnkkeedz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hnestwqz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ihwheofk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nycimihe.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dnckhphx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3goitxjgy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmdzrmdk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3uzembghx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gbjflvwk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3svnefskx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yamdacan.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mhoibpmz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mircnzmr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zhggover.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kmdoiktn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqnwfkkz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qubmhwrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wqrwidzn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3avgayvie.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mtmynvxa.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cgmnjojv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3toqjbkdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ulwjptaw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zcxlwpnl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fbbdyyba.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pulupugt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yanipmtp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rwjhkapb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ypmrryza.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dejafgvk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lbxlofbr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gmzsgwki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bgamyrxu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tumnntth.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3smzsswoe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mvzprumk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijpbxsxc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lpfdqtay.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3athrvvom.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rjpcghuz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdylosgt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nvmwlmkd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hltoaxge.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lfodkpzf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3chbmeubd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3augejweh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3czubeozu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yganuskk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sqrefxgo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fkhydcwj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3adtjvueo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pjzohxsm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ibwkzpft.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nuvzduqr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kqxivtxk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jjxvnyye.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jmgsrele.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dtriwvdx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mmdqoyvs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iizalequ.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kgjjioax.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ybzmeceh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rlvcfooa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsmuauk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ofyjlxyf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wfofucnx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aqnpgflh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3glgqdaze.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3efhmhrap.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jaygpmsl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3djwzfylc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3slujobsv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3crioqqlm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3engemrxf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3flqasiim.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tsgitgcv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fmzayhpy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wkhouelc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qufxoevg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3llhxghhr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hbouetes.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3chlgwoys.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3frnycytt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qeaoauya.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wbgnoesv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3icbliqdj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rupqycuq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vlohpkbt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cfycgist.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ghzcvlmm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ylidclkj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mpxxjcos.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qiubfkvo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ntywjyeu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3znezxnpo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrymlqae.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tvprqvds.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3shhrsujc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dmozbnoi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ofhjalfq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dsamumxp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pgqajwkw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hurfqxin.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3sfkxjsut.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kwspskpk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zppzgctb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3snifxgdq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbukbcc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdaatkpu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zrsabuva.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lmuyvvoy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jjxynjyn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zjwvlbko.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fdwuxunb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qlfcpmfk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3nkxvtclx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zpmwwdza.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yutrgllx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nzsymliu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ibvayyuz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ivbijfxo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qyfbivbo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ougtzmhx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3koqofjxf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wwlyduao.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pbycytqb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3bhertxjx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qzhvzets.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmpfwxoy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3umfsgoci.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zewfthxf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qfyfbvyi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3obpvrbma.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vkiyuqqy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3axlhdand.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ebjldnxp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3prmbomyz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3joxkjexf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wvrxwljm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uevapnsz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qwcrqyac.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3spaimlpw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dgualcas.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ufimirxp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3oelgymel.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yzmpjuuf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lftqtfeo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dxecoewh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qpktdedl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aewgbivw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ezskmdqf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kzucaidx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3faxmukgh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kwnesqkk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kdypqodz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gxqmkyzq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkznkol.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3muzjqynz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pigqskjy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pbtvgrhn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkshxno.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ubzptzyl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtnptei.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vgvfmugm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wvymuoqq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hgbrsvaf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eaalrhqr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jjyrgylf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jtddnmlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sabmtpcv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tstvvdte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsaiiqjq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3posanyfc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ikfooohr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mzcgpwow.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pbukjaee.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tybfrabz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hbyuthdw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sivgiltx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3reozumrr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rznsguni.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xhociibo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3obzbdciv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bdlussav.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ymggketm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bqmzgaky.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3uuzirhsr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ohufifky.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3vpjukexk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xazwtprh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uirxlxxg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rqvlrjsh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rsybtnqw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzsvnzi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gexctdow.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dqrzrzck.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3tnhqtdji.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3obqyutmk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jccexjip.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3njwlkgec.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hxzhzrtz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yimupejb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ybjmttmd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wtsuzled.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rbeixfgf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3kkupbpxj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mjzmqnzc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wjjwmxbd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zdrzpula.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tovhmzwy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xtzvzpqz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3dlfjsubu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qxwsplnd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rlavspol.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tepvlhye.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3oiusfxdk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3lrnuoszd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ifqwwyxw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vvljhmvn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bjmwthsd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3copagcur.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wcmrhqtc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3eytolktt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pntjfxyh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3slilmbof.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3cvppcwrk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hjpcyaqk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kqahghrb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hjdiipor.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xjjhsfvt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jxewbrcg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxxfbuy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3exhwhgbo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gwtisqwf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vfqkmksu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtmcle.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3yntrllzz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3imzdgyer.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ekhtuenh.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jfclrolr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3brzajqze.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qyoywhga.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3phkqhkzc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjpfenx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3isscnrht.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kdxkfpzl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oidjtqfh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3odtyvmvt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gdrgrjqn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jrseiotd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3iglcnlcg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3egdvxtjr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yklhqjzl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tfokgkxh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tafpojwt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjvlfird.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oljyljbu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ibfnbiju.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ofovevff.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pirzygut.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwhacxog.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nppkpzov.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpvkcspq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vkvwsjmv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fnnzbcxv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bbdypxll.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3raojhffy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ltujoemf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vzefaroq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3upixjlsr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3syaagxql.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ppmsosay.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kpqpecnf.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ipyaqcgd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dmlosygh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iqluzrtu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zjmnthxz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jtkuoliu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ktnubsei.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3slmlmmgi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ixxhyuer.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qayfhzcf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3enpdoiwf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gcopjffx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jvcsmyek.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bqjeinbp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uerbegxy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xjcjkuzp.html


<!-- 参考信息 -->