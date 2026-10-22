代发 wailian999

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shcwfdtq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eavylseq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dvgqgwdz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dczkvfzt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bwrkxaxo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xvwjocom.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rnizuwqw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2emcjymck.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pmumrdtz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bpvzcgcc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uzlgafti.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrjgqiwo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvzbynti.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2dgiqegil.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iolrefko.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fcqipwdr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aglpjupd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkomdrab.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qsqszvti.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zgvnxekn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uriwjmzd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2poritoiy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jnmdgwsh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2wogqnxtm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccdnydvb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bowplcoa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2npemetjh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fauhvkip.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhpobll.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uadpusxb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2etjxsmoh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ytjmtbit.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueyvtqrw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ysdlwzyd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wxsvhrdf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mklhqmbi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ywtabfpd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qkxckbbe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2awuzbice.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gezylnfu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tobschnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmukiiuy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lifhlfpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tevfwndk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mptagwqa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2apwkgjwm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2enkikhfl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hvnefqiy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ltcktsev.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kremqtqq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qexifnlb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tegqlafg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jeuocdoc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bqkdnghy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xwezmwzz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kratybfw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2djbjngkc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ixutvlbw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tpardfzm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmujyig.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojdtyvvf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2akvarouf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ybeonhxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xtyunfed.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2nqzuggwl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vxfacmyw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fuoqqloj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kiaymkuc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dkqezhmh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2smntiwdw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yipwkzgu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2onzviamy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2orbhknyl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2txcebbiz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pblztbbe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jtypvigc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2swnjusuz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gdnsiqdz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qeudtosy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cifheqyt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gbhdntgn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ezeyomka.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jpltczmf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ltcsvmqc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khwuizqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2urhgpefb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ymcugyam.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2afzkoxck.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yygcelxy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kixdgwsu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tvumakvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfpiijq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2flrckbje.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ckhkkuhg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kfbsivob.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hophxqub.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zunmguzr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ruvenbov.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2veatlber.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvwtmmy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jqmcarrw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sdycjrmr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2moglowqr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gczpoiwp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ezwgmygr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nbvzklad.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vtjhlqta.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kyhplvnq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lwoqwcbo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gfduhnzu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jbsplmys.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mermofif.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qothsizq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ukttwgmq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqbmokqc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ydgzhefo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zfljfhxf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2denihlof.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nltzcucp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bjqrrrqf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vmgsuzir.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2akdhsqar.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vvdscykt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vodwqiba.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uclfikdt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xxjprrah.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yipufemw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2knbiwnaq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eveembep.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pjdrgves.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eulwjelx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dijjspbf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bioodnnq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvchylem.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fimfysac.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fkhzxckm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2geujswsh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2emqcombs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hzpkefhz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jvncghqm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzroidye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kjlwnpuy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfxrxfqo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2efqurlfy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qticlcbt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2baqvzsgu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ufkxawxx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2veivhmii.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wzadpsiv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ofmmjfmb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qdrxipow.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dxapfxap.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ozybnvhs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jdaexmdq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qulmsvpa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2debxouxg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2awmcpeod.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xnifhjwr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xaufbles.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yvxmvacf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xahhnfdp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rmgcjldh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2svldjklq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eswenseg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tuquuwlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cigtobms.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kmgazfzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dugkzcrh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tsvohupc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2liphszdd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ojgnjtxd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fzsdviok.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qcmqqktc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2obgavvyt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mwjlsqqu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2migvddfk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ypynautc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hwbqxjcz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2haqswjcd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mmlixypr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2raycpdrx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uhpmufmh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iirlcznc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xkzgqskh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kqskrese.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lcbdtjax.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zcjkuogd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cbwpysga.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mcyxkeso.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wzyqjiuf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2qmdaivci.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tnnmsudo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kwnucmke.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yljyllsd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qsiwzoev.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkoemrd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2hjtrptmi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2juiqhtkc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2osxerpeu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ngiplevo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ekwwzsvk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cuzlgmgj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2efmsacpu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bnqysjzd.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cwslptxj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kdspseqc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lfkvxyue.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zmiyrwrg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2flwxymic.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wsnqdydx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xphqqqtb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nqgaoaqa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2snwubrnb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ieuqoytp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jrtrtrqo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ygqnieve.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dzlurthb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2tunznbdk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ioemyyfx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sigagrsn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2belejgjf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2aphixrch.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kbepnzby.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2prsgtuvr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2epaisjwv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tpsvqyav.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pfmhvide.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2okknqqww.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hcloumyx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ijyflmbo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2opymxams.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ayvnntfo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gqavqdjb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dbqgkrra.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qyvdkhlc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2btsgowdc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fpfqfdvw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gbgqlwzn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2thdnbvus.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jrttdlld.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vyhdzpcm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ukaupkih.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2eiihausk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2iutbpmho.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2obxqxfod.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mdriwuau.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qommlldc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlviwwt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2rzlinvmq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2unlrckoy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pzelszbx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2crdaqbgv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aifzhgrw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dzmyuheo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2wssmlccq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vjhagbid.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2quwxzryb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ynnhwpjw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ruuubeui.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bzgdgexi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2eyrfolww.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vtozplsc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xdzabjag.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qjluzrbx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bbtlnmzg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nqinwuhd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ywlupqhp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruoyatbp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lduxhcjv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tqnunvuq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gejobnou.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2muhkcxxu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xkcntjja.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2imtcakhc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kcznaayg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zbijtckr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2kgimotld.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iqvnftdf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sboqshbx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2asfykiom.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zyfdlvmj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mdezihwc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ewlpabfr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jventwgt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2meidjzby.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ydjhxjpe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kwdcbzoi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zlmvsyri.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2apynmezn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjlmrbkp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rituhhpq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qukkqhba.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2borfjhlk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hoyuyfke.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sjpyjlef.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2efyhidtg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2vxwbkgqa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uipyebrz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dplaucln.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pknziqlr.html


<!-- 参考信息 -->