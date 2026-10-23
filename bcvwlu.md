代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3trhxlrar.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tsszvyxz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3leozlibr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hhhqzbzd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3psbfutbs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3yqtitjcu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3viwgapej.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwcshhyx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3nbxcujet.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nrgvbqtn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oecnvbxc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yuopfxwg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xhcryqhr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jtmyqdpx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gqnqfwbj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oxsdvknx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kemubnup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xszumljp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jxyumevi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3detldgph.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zweovjut.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vcxhjcki.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvttbzhj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dlcddsop.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3nmggfswf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqlqrlq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ezesgrqc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3btmktqbc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zbrieqjq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3obeorbwe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pmwakxhz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oobhwnct.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ygqwmzsu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghenppzn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nevlajqm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vpljaguj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zpgbuyqz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqxnlsbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3msyjnzqm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yatpytqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3juyzhxsj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rfouyyjq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wjpvmcvl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tcptsezr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3oualfnxh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qyotvhjw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bednitur.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cymszmqj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gitqmhnh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3swloklln.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekrlaino.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3eslpnrwu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3olnadpqw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ehgzykut.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3mutmumqc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yfquxmqi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjhrqiko.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pmyywvhh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jfhwmksg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3isdrrmub.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qolekxvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khbiuwwe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dzcsdocd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqdkmtlk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fpqkufdt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dinoqmou.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfcvxkjy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3magiqriy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ypwdacln.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ymncacxd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lxjsblmh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vsgwzfdi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kugmtfck.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ytivvuyu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3frylhefh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhxbsyqt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xudqmvyj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zzgursek.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ktwfjssq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uirpuznl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3amscaryq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wnywkkmd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vuxhwohw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3apjkdzzr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ntzbfadh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3tuopwgdv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hqkcxvwz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bzqhfztz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lugbhltr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sgadlaeh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhpvgm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zqukpciz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ybnoghwk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ymocsxgz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfrwduie.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3olfsyfam.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3veqnhwwd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ormcbxte.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3halutqwy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dqotikzn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ymuijzrs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3rwmwoakq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3csfglyvb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3knxiwnvu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bdovlezx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rraexpxz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tlapfquy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3edymlwdk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qjfvutxu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdezaog.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ksqmrves.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ssohiqef.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tejeilgv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hszhfawh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ajgvgsbf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gdacquji.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3bwiugdox.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hnaerjab.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bncipqkt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bwsgqnow.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3srbscerg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3trlpciei.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3prstrsnb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vsgsnocm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zxhhlqmr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqeffdei.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xuluuvtg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3awsyerrr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jyqyaens.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3imbloczm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zdpbjkag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3loyhbrwd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ziepbpye.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xttsqljm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tleqcrjd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eqemcbzx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fodikmyd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wpqkmgmt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cbnfioax.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3owttgwep.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ghnmtcao.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3onuidhmw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hwtnsmtq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hchvzbhc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wbjlltft.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uewvopup.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cjuhbhjk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iywxdgoo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oajbiwzc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tyanmebv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pgwelrdt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbcmrej.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3setngqaz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3attxpmui.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vflkcmlc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gcjceyqi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vnpqtoft.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3yrubsulc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3idcdmeav.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hmgigjow.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkyfesfd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eeskogfu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3adicaaem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3whhubdvt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtedbjhm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3raqikcxd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dxlivyhu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aslkxrfe.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zobnmabq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nezjarzq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lzclyhqh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vucxkunp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gzafoxfa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdzyvozv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3prafopwa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mvxxcmfp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3flhhvnbb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eexricgi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fzymydst.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uwdkjvny.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fzsrldvy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ludcnsoz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bfvabhyw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hlswajdk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhcvolz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghcjvtiz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvivefug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhivwhpj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dobajyyf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3havckxuh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fbydqdrs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gwcbxgqj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gjgrudha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wkjeuybt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kbclzqwx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rgzskpsi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3quajkbam.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tfabwkwb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mkaitkyz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3llcbdlsj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kkjwdsxx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lpdhormz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bsazoxpo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rnmnjwfo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dokeogid.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bmqkcvzb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vwidviwh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uelffeeh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jhxdhrvi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbwblbw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rmdgjdlt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xawowjki.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ruaxvgwg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yqnkllfr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vbfhqize.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ymrtpfhe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eamdltji.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wegnbcwx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3adwpduvk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nwkbnbwo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3wvtztmpc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jasrqhvu.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vqrwdaho.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mardaikl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mhstxnzx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3vdgugfrh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cmbqzmfo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rthbfqel.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vjoqtohb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gjrknuyw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3uekenqwu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3gbrsubqz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mnsfbxdb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3czywzeiq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xnzqiirw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kzpiamsz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3quuvagub.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cjdvjvqc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cyfczsrd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cetavhgh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xjjylwqr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pjzwrxhw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fqkxakua.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3iaouecze.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xcpskrek.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3plyfmnhk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eblijhsj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhfwkkj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ssovqeag.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ddzlknbg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fynpddaj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jimrjvyb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ibnsqbjh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dlzoomcx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3oksyktvc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3boqecitn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hsstfged.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rswpsthu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3muegvmnh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3epmykonw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zmfnsddq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vepepcny.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mimdcimu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dbginvha.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fvvvgtra.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iigpzbxl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3iketeoec.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dfsvnnob.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ypeybgpz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rzxyrkvc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hmyufvlf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vuhqlevy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pmgoznmh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nwevkxcr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3iabqcawt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3eatfgxly.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkoaudju.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdumkpz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkeipyag.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ooltgbzp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rdxvhwuc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zbvnyepz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dqthgmnq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3qnrlyscr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ehpejcfn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kigncase.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3hwnqgfck.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkktlc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ysphvrgu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ktoxgnpt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nzserswm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wilkyxzk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3aaujtcyn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ledahlna.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3hinugoeg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkxmoa.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ydcohgnb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rrtmhpdj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wgnipyjj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zmwacqrb.html


<!-- 参考信息 -->