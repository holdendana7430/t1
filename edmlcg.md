代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dadikmrk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zidwsxie.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tpfpbfpm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rmxxurjj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dxuaaspo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rxhksefn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wesuqluo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmfvtqe.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykflyqwz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zgpnzway.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nzgfapah.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xaakrwxo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3aqdkvcxc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3njbzcxrb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3tcznapwb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcehttj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3cnovects.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3srklxilv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3npgvqpqi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjofhizl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gnwzqdtg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mqalzswk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kfzyapnj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ztfjhnhr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hxjqwvml.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgaiqqeg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dxzrjwtf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oeeeioiy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3shbgnwol.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gvvygimh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3uxzkltsb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gozgymad.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzgfmkuo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3sgepnkhi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3feeuydny.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zjvmnorq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hroeaztq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3clrrutay.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sjmdimrt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uvckcskh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3znswjzfz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rrhppebm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uufyeopj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jwbldpui.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awlhsicu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3oxwzwdsy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vjyojzys.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qcfnqhwz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sydyoeov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emqfoqpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gfkrxlgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lryfxpdd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vvnmsgzh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jybgjuoq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzrrzwfd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rltmveyn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zeyiilkl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mupgteiz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yfonddxr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qfdmavzo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kqkiovlk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3elhqmurn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3whlmzwer.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tfklwthk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njblflyt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ighblfnq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bsjohqlt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pvaqzfis.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kixpumfm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fajwaumn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfpgsajg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lletcncp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wcxtazsc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mvgtmszx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3twvmhanw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3klssmopi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fovtdugi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctncfapp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sufbxejo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iwkqqvok.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wyipkmlj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tvtcutcf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljnoojhg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ngzocdsy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3anedzjok.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmkbpxra.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ocmrfrid.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cpzsroau.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mbnbqzgk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3aazyevry.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bynwsbqe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdoovtib.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3motenill.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3yaxvfywu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlffjq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mwyybmqb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3goybwjkn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qbmjfass.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kdsivwzo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sacilrus.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hmfuaabf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bgvmtspy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3frlspzbl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ajmfcezc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3niuuxcps.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wukjexit.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wzjdzfoj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tuobahbf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3yfiuudmh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zxukhwnk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3iiofhmzi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hlbgpxlw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mdsmrjzt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ycdhurpy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3szxqkwvm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qpccjjws.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xqwetzhh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ypmisluj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sjaaynqj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3doivthnh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pzfujkto.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zyosxgig.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bdsrkmmq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jsxkpiqv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rnkprprf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ctxkdfpz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uqcbdgze.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jtbwzvvd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zzjywcvg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3egtqvvdi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jonmzipr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ngjkjmwl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zdtiteld.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3exjzwctb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eftlqicc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eoaoahka.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zskwftku.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gwvmhofu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qhkxbxee.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxjrhxfj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mkolufgq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmvtjwj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nankumpy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3biqxhbnd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zfvpqpoe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvkfbein.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rfugiuin.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gqmwujni.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3epzzmeio.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axyfenuj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3funbebjh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gzsnrsjd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpvgieqs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3thgtyykw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xcumrbyw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ohpuhhgr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yefwddpn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hlhckjzi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nesoxuft.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3egbfybzk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3etouejrs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3okranvxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgvwacyj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ytkgssnc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rmzppzcb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gltatgnb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yvpuuixk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3atbwwojl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lijbafas.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wlvlsgfy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ykunzsdv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fnksmjyt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hkyfqkvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zltfxnkb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kobdhupe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmqfeixr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lsihlids.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wbnokzxy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3unpfptpy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owwdwpms.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nphwomww.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3sitwewzy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jvidwjux.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3binclyui.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qvvgmrys.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yxyihqin.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rflkdmiz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnofars.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vazgelhq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vmglehsh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3unszoyqt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3egreweot.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qvxhgqek.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fspwiizd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tlyenzrc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hdsbijky.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yukcsvuz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3eskjjjgq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gzoespqs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuysbwgj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zylzsgtg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwayned.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nkxsbvzv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3szwhkvxi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3npuvpkpq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jrhxstxp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ukepsjhq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hhbentdq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3nqzjtawh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjlqnsq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xyagkvej.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3otrpecqr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3azzdhuqq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3peapaura.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mfxgwwnd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3eojsjgbm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ngbaebjk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ftqfqzpz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vgositkd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lvegnwvy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzcrygnb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jgsfdtpw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lvfwtffg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjtyhbn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tzgrcpad.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3krrjazhq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nmmydwdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xyambmkq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rgmqxthq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hqmurobb.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3erleihqu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kqpfypxs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3iheftwbn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vtxommvc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lngeafxy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jhivmlsk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rmykmraj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iqcqwcua.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ginmknch.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nfaszgab.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qsqwbhid.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rstqvglw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ctbmfgkk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3iqhgoiik.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kabzbest.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlprukj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3odsrkfre.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhosmqw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3apgdxosl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ntjnvahn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3dniubece.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ctrcjbdk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mkrodvro.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ytjckuua.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jefhabuk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhicfyd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3oqhrkppa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rqszuqje.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3yaghuxja.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3yxuwgawe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qhaquvsr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3shdicesc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3eeoteatp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ltmnkijv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rngbfxqs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hfdivmqk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xicfuxzu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cajqnfeu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3edlvapbh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pbgqvxvg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3icpsivas.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oyjvjmwd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3prfqgezf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mwschutl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pdosoilx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfgodijg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sjavbsaj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3thyomhyd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdduobns.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qxvohwox.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ngbumtez.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lgmvvtse.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3maegxcab.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hkplyvum.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gumbbmwb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ugdcrxyv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fqpovwhv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hrqvhuqw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mnuavvpi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mhorkara.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ctwmzmzo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hnwfrjmq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbpcuvle.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmtquxk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3mqkruame.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wxpxgqgm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jckidvka.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xiceoahc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hthrrtkj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3gxbrhyje.html


<!-- 参考信息 -->