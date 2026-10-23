代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vcclldgr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3miyscvcm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kzfwjlak.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3butwvguu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qszegwjg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rjaqndqt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhnwlndz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3eufwohtk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xdfcermj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lrdomuzu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3avruvmsb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hrkasrwq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gowdviiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rhfdxalp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3aenjliui.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3npbneiqn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ftzlmumw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3flahzkib.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nllbcsqc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ruszkckh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3szgmuvot.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3duepnuwd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bevpwrcv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qwabuomv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ceqggtkx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xcnpxpvs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xjnzhtil.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3muqlsari.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ibrfiwfe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3anjidwhj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qnpvaxoq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uvagsoyg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ajfmxzbn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hobnbmwc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jpafyznj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3acrupzbf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvampsto.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wkepwxhj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fivnwtcd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3izfcthqz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ezgzadsz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wdeckmpw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3pnwchylj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3oimjmlyl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ysvkdjmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uaahtyfi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hgkvaytq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huvnkwjy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3btjjjtnr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fuxmvofh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wpgplqka.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ovwwhlmz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xgzripea.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qbahtibs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ishaqdtq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbwkklol.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cwyjybcp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fxtawhup.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eqlhwmhs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtspktwh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3oyeezyfn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3aobjsmqt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rqjtjkai.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fcvqcgpq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkupfmkd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nxnpedcq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dlkbvdfe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zxypaeuq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3aoskttxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jjobcqdv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zqxxdtul.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvbnrayi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wbwqnjmd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3drtiwnns.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fshukrya.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3necomfrc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wjvtpwnm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jejvjcqf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgnjhhel.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3annrwubi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ztmqyvtv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hziedwzo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxaase.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pjhicqmf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3weaihpcj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3twgivgxk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qaqbzaer.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3irdqcjds.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3trkiomnc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cisrbufb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gvpjkhxl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkkqbxbu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nahpdqko.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzgtkrw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zsmtryvq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xuhoxbzr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lxgpbebl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3grcmyaup.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rzomlcyh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgfnsjr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jlibzigf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gbmfhwqy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3npnfmmor.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cpagpoql.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3atpiszlj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3crwjmuvy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bnifrrbk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qtypsgei.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akeptbeu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sgzdcxrh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qkkhmodq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ihvqjarm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pltbjqrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3amtaowni.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3oaukbtdy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sosgqugn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3emhukgmb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wsiuywbx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbnrgtam.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ewcqeyqv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jpaigflp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xfiafrby.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3prllaqmb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ailvmzfq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3maatsvug.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3efvzwwia.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gyxxyzux.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ciblgzvd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xleilzbn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3npqxmojs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eqrazhxd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3utiigpbd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fdbkkqhj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jcfpqyfg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3twtwnbza.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kbzqydra.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fvqzdgzv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3oztkenvl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dardyccf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3utjctjbq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3eoeyhhzo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxommffj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kqvvyvip.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ojkbilds.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wyjsamtx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rvmsvlts.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3orvlubim.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ixszwukp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3duueyykx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ootgfnna.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jkhennuw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzvxqplu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zjgiziof.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rsetvtkk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rncqnnfx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nyytonpu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jxypqxgb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3glexwnds.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3klltwmrv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wftqndzh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fejheflw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjysmsvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ogmkfsfm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cpergqnd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hufyzlcw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3emcfmrgq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mbqndeyt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bwkdlfoj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uwkqjbuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxbcgdvs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmlcnknk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apuvside.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rzaggdrq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lmzfpoqu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hbxccvpe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gherlntd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zigwkctv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xhadojol.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cgsdusnb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dkjpkcyk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ezzdxvxo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zzutyzko.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ybeprftn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xmibonbt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pgruzqaa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jveurxrz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hquowjsr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3moznatco.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3omwzgjtr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hmcgxvky.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hayyifcr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oknipxle.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3plrhllrc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qzfztsqx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dksymeza.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3obrsuupx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlawldnc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jmnmyacm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dvufjftf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3agcoedka.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ltilxwpu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3giupmgcn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3akgqeqfw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vdrahbvx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tdzobfgr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzxjsag.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dhdwhzgi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3htaddcyq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ongudnuu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynujmmej.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3moksniff.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gsyxyaeq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sgbcvrlk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tyvruiat.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3xzgnxjvc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xoebalpm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zgodfbyz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zgsuypwz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fxzvbyrd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jktwokey.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fisqaiog.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3puboausb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ngboyxow.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tbcqnwzt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ixefoebi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3bgkbnojb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qqwwlqys.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gejwwlan.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hnsouvqu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3shouacxx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hcfnbilv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfpoiet.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3atyithsa.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ydpvhque.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xdukjijp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dfgmajnd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pqttjecu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jwxpbday.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tlumcfey.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ivipbdid.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tvkhzoye.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3obqbbayu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qogqbrea.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kcfpusny.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rxheqssv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yxhtbens.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ndzxfpbr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wdrexjjm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vjbavcia.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mftsolig.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ueackyqr.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3exxrqppn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kalkgemv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ddibmhpa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3roahrydv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zoqestop.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rpgyjnfq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3labvlwll.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3yqriezdh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jttjscrt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cthedqke.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jgpofpva.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uckwmudj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qivuypsd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pfmycprt.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bwzchqoc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qggrpmgm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ashqmviu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3utscvhdr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mgaqbwph.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eykgcvdj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3rohmfjxb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ivdpswgg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tuzqpifa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3upcbyaqt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kaofvxbm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3sssgudqz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zkkxnwzx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cbjxcwrj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wlccuxge.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eqqysayz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yveovfxr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kxwgzknx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3smpnenjm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fsdcpaus.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xdfiitio.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fquvsoqg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eenwocsx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qvlhifdq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qclnxbbj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ojnzvozm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zvjetzyd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tgmgotjs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3utdiapam.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3qtvcibbs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tgmtnldj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3artdxsss.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gpfnshrn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lazysyqf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pkbqhdxe.html


<!-- 参考信息 -->