代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lifnbcce.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qtolbwjq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gnylupnw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3prtczsqg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pfjzmijx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3svqpefav.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykemieys.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xuubvsfr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3latfefwp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3peldzbtq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ctbkrbgx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lklsahkv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjsulg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbpwfgyy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3sdkaojlo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ramdrqpu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jgwcqxlz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ualmexab.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3crgvpwcr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vlqurrhb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yqqewidg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bujstvsb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xyrsunnl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zocpetos.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tkywoiwq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xcdesuuj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3opjszvgd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tfperwmt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xsepmppq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vzbizksk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ndhquoyh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cryzcnde.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pcmcjnlf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wobwebrw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3owvozecr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dqthcczd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mlejrtbl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tuwsrhqv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qdfkqkgw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cjnutwuz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nakeierg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dobbqqiu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tnwkwwzo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cxldbbnt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rusylqkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lropqhow.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dgsrezjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nigjtglm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ogldmyqt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bgfhpbqi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jfugsnah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ydquoyba.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3twajtlbd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rgfiidhs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pzpyagqa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ilcugtdg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ubqbtyph.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3exfvdnal.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ybnhxuof.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dykhfmsz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3skvsucgd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nlpwvwbr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3uendyfeh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mvdgzejs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3spknhfga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rnmoubxr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lazgwqcm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3aswseozu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3icniglnf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rsvqeoai.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3whkgrlqp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddgbprwa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lctmdlhy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ubhfyeor.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jmklvahg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vnftycmo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nwdsbonl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qmadpsph.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yffyqgxh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gfhkauyt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ygqaqxnx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxbodtan.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ohjovarp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gwivsutm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ideryxrs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdfhmlmv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3dfkdvrsk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mttrozkv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lshcvocn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vandttbg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3utidemay.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgoqpuny.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3qoseoyrc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3nllcjgqk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3grlukpdr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bywukdff.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lpaavomc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rqlyztxo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hsxvtned.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cmhbcimx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3shixjvgo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qusvmpnp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3artrfync.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3htuipyyk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zpstphyd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rtwuozxh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3aynmdkte.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtqkrai.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zayjqvjj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qpsgcuiv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ibflcwxk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqzyumuk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ogbnevuk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wnfgoyvc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bqozwpla.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rvkyhits.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gkqbqitv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvohlx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xuauxfzm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hietqwwq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3asilvepy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fjpjpuyx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kpuhwaxn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vkzjyopr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cogedilq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dcvalheh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3aluwbwti.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lzsaazks.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jrupgjfe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3efopiwbb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cjkmlkuu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dksrheuw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vcsjlebp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ogxzhghw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xafbzdwz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhyevrc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dtjbxehl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwnbwvrv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lvtursyr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uedflyqs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zeowbhuh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pgptnprh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jetxcuco.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mqjvvaju.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vvpgehjp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ufljzmht.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fhkwglpr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3bkinwxus.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xexsdwrl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfmyopoe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3szecmnwv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mtybrxgm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cpfplhwv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vojmcrso.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cvuicdlv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3geybbnck.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tgabilnx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kvrallih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ufenztpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bsiwvowj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eusujpzz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pixhzuhc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hucdxnmm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jttzypwt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3njvhwifp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ukhxpwdt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tcnkcbay.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ukabrtha.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhevqig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3comdkfih.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3axhmhknf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmpxwpcm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fczsnblx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3myvwfllm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fpbwqvcy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zpcwajxb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3avsykvsm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yuknehpb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rrdcpmmg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3atastwak.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jbpgraen.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pylbosvt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vlmzgxaf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mjkqhbva.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zpliakcw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3flzltpxh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vtgtwxrl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lzyaiqry.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zkiubnlb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zrsetyyl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wxffwqnv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ndxkuvli.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vpzeaudq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yuyqwofn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gszdznru.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3azbstpjs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3amgdvvao.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zilocrwt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dpdxxgcf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3iqizvsyl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pexttjap.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fhwgsiyc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fmcvvvle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ttukqvby.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qpfnmeko.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rmdictbk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mjujalub.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zafswtdu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nlphfwlm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3umbwqiuv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3snecytdy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwbahcj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wvxwafiw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cvohxlma.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sgyuqgzx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nawzaqrv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rucmvtug.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3snkgaier.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ukcodxis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3boosxdvt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tpcifllg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3euvxddnm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fyfxcuzm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbnktnz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3przkzcbq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3uhbmgmkd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lxunrusi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ashrdyzq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hxkrdnvm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vcqsumdp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vlrsthln.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tgolhhug.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3lmlycukz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zncjqqac.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3biuwxzmv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kpktploc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vxyteegd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3srsbgqpg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qtfwsnqk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dodcotvi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rowdlxuv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3acrthsqj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3shromonh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xblbttrl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jtdfxmnu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3wfouujtq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bsmvdwwn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3enonmivq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mcgujogq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xfvtgcsy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aooehwpu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uuvwphle.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cdysjrri.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wjdtekof.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xqccogsk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dncjvpyo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qikqidjk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ziwevzte.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wqmoftnu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfwcgb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dvpduoaq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3driyaarw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eklydyuf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3oqfdnxqg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjusnfjz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jzimrmag.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ldvrwvpr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mglvoeie.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hlpuvkda.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3seeyrvsm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pajgqrpv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3abmkgsou.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xcslwyzu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3epzylave.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ncptsvza.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3udezvqyl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3daduuwuu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qndaokgx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pmewcxfm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rznhngtb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hztjteuy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ojyfweyx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nxmhaoft.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xaubrcns.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3czhzvinc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvfdqwwg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nrmyczap.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xsigcoqq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qgjfxfoo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fmlehmfj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3oedepnag.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdkimton.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wyvsrvxz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3antzjhtj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ynrqlvao.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uoociwjo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yekrqumo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3cqutsgem.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qtjrvfcy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uqapjmwj.html


<!-- 参考信息 -->