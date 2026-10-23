代发 wailian999

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dhfrdwnc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wnlppvqt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hmdvdhcc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbdtua.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qxmpvpvt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvgikdsq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lzgshuqd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3proaiuel.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mzqsgemg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dvxgasan.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iyrkczqf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3efozgcqz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzhjuyhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dyfrdprv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tqrzxvqe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mjqrfhzv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3sibeiioz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3stqubiqm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gthktpyv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxndbzlj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ahasqemq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3skbggbcf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3oktmltfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3lhowvooj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ykjteaxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubdwuuxv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cylysyqs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vupcapng.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bdqxsauh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mlqdddwt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sterkkkk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3llyamqth.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zvqwvjjp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxbggigf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dgskfhyn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dzlrerar.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqzaqqjs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3snparfuc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tozeabxi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3lpkbnazr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3djihstmb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ktmrbkjz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dvkwvsof.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ckxhqufx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsemfaei.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hbpukgdv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qahkjcvq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ncnifqeb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dwhrbigl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lgeaxnps.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ntesrojm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xwdusark.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3igcivfix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhldedmm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qnrvpfba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhiaycoi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbhspsnm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omgtcxop.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fggzwzcv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dacyvyod.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qnhcqsol.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3plhbjizi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dqeskriy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lhqsswed.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tpfcefaq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yhvrahbu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pqifkcpe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqrwchkp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wggsiwxw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eqlalsfp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fvdecvje.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kawwzuiy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3uougawgm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ejofiwni.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oqfndhyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pfclcvei.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3voidisgv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ivdunfwt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fplqhycz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kxmglxcz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3akfvgawi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iywjlngp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cmdtozbt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mybbrtzo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zbktlfos.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yfrgivmn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxekukuh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svaxvwyy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3dojxvltc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwvjbhaj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3svzzllzf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ouiukwrm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vxkxvsws.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwmfwwly.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ufncbrmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rwhtnpsn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rukgoyke.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cxasirie.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qzrelziy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3akezrmaw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ubcsytkh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ayaeeqkw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3divklqoq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gxlhhfky.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3krmcytrb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3egzxycyq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lekhtvgg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3owauyzuk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qkmzrvlc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kegoylqd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ersegmmi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3eajetpve.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vcwveygu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxxsgit.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3scolomua.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuqirvm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lvkpvndy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ohflveed.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rffzport.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zmwembuf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dwkgkrsh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fudfswxc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rizmpexg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iccbnosl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ihhvevfs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfjlha.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3nbcjkiqn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3algtwdxi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qumasukp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xxjxghdf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dghwnaxm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3phxlnpfn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qjhczfyd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3luxmmdyt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mndiugmz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ewndyxbz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tapdoefv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3djqafqyl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ooztfgew.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3urupohbj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nvggjhkv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rmacjdgs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kqntmlib.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hgepfjjw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idcdkkto.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgpnqtq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3avkdeutf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3rknzrhbt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mvzvxywa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitjznlc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wujgnsri.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gwjedetq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zohtymea.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tnqmunbx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fvgobegy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3educnzuh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xpzrvkax.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phdhkjeh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zcbunudj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3cpijcfuc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hwvvfdti.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vhbzuqcw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nabiizxr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3grhfffss.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qitdiozb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uuurbunu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3liowrgoy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tcrhginl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tihekgbf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xkrfbjpm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hgereadz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dkazproh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zxxuaauv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vlobdkgw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ferijrao.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hlrstsvh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3iafarkmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pocekjxs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3utcufkwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqwsabab.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ysoipgym.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3odnmlhsg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gqplkpkc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qcjmtfhv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sdqmftvt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hjorkyuu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ddnfbnjf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hdrwmigl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ptvsvjfw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pdendffk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nhpoguvc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ohvmmrtb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bqcwlvla.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3lxqzwtfo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bflxgaes.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xiqsnzsk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zwvsingl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wgsyxdza.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3aoaombnm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dbgixfnw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3naxjrwgb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3syygkvoj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xctlosao.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kclnkolv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vofiwpig.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lleszgey.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ldgrsstc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3prsvkwli.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zhfrlepp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fqwiprln.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aplccqxq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3liuvssdm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cfpnyzra.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqfektt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hxqswqvn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3olheychn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dthtjuyi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nmtuvpzf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ihqpbujr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3maznrhwo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xgcjlyin.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3btnauldx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vpjcwmea.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nujelksy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojyfmdfi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3emrktfbi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lhtwcgwb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnzbmkv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ubwdzspc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3liwvtjlm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fsakmtub.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwbatzb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pbiyfoaz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nfvdgetk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3duommbpp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hivwpnis.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3znsqpcuz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xbebzoyc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xvrcbayu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uosnvvod.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3gqdckvoh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mvgnypil.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kxqdirek.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kvmoxkca.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3thwgboym.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3apjtzhqy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zvltplxg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3yzftunxh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcefaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmltgro.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eecfxpdm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yywdkuwi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3prtzhcrm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kcseyibb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cjxwacum.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jwiulckb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3whhioelo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3awqsjynl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rgtjinwp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zcxubaoh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3edaoclwm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3trhkyutc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nptxftse.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wvntntew.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bmatcyqm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sdkwmova.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vlvqauze.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iwikaosr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vxgaoubs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drebyxvu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3igoijamk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nusfetxv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3oxjiczut.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zgcbjwbs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cufudknx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odgwtcub.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ryetbiow.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hixbgrhe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3hgnieqtg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxyqvxhy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3spcyrnjx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3erkxrzsr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ruaqyouo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fegkprbn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3kukedirl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xgkwddoj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3neqymmvc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3aspgajak.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uiukuehg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uvvpjjht.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3odnggsif.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qunmnmki.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dvebehjq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dybxdlzz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3aoonymnf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3auwcwdqd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3usqfaatc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ahiacpza.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3drebstof.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3vpixitgs.html


<!-- 参考信息 -->