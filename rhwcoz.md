代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dqcuclme.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2taeelmfa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tuhkylvo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iaqxqhql.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2eghbfwtx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xmzayvye.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yikmpgjt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xbnawepg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vdtnggev.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wrhgjpdq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cdiqvvam.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2giigglok.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2sldbydqm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hlvtfgtv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lzkehbhx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqodfsc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxlzzpvf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zdklvklu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovylkomj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gyjctftm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2uujhzkgc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2psysmqrd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ttqpuvug.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ptaxvtkm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mtacbkzs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lvscdoqo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yiizthyx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kobkntte.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjcxaxas.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nzwudfcg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2kabpuilr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uhcwtbnj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2spezahds.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tidxizmk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mrfsduse.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2itnzzuoq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkpcsvdy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zuoaimbz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rwndyish.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qwuuoxjr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zjwmphhf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zehawgku.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2odprscuv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjelpzfo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pkhomcvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciizbgqs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tdtcgasu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bowihnvh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wrtpanhi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qqbljhuw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wqrcodmb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qmwnyaqu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2oxxhuuam.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2slknaxro.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2obovdcgy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qfrkobet.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jqqocmkk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rkwcfvis.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wsjvitmp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fbnklezo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lxskjjpy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2fsxcshie.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wcoivoos.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ktmmpeow.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwajuriv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hkwlrekt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hndlmooq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pgkuhudu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qexvfnib.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ezpcegen.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2olcmkyae.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kokclnxn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tzhfvqtd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qatrhrfs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2duuaklzs.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gbssemkn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hzmimiue.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2npiyuama.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrphpbbl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gyflemxk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vjxngiug.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuaomoow.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kwfmfizl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2buzlhfqx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gfdprtej.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ekarqfyx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2suoanvcm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qwfeomva.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mucwaknf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2piiaonht.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rjgjlndn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rltvfvum.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2taxehgyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mdqthrwc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bmqohfhw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jjuyphwj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2urxofvtr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2pxqtucwt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wanasbkh.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dsgltdci.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sdfqrphp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hpfakswd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2avlsvzlh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tyysdoci.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qhlfkinr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pybmrizp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dakinytw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqhboqi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtaljqvf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mbknraeq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ftqsuomt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hqzzncln.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fhsqzrop.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2scfmlqcn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ibbkkpcv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pupmdnlr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2onnuiruk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mlssctnu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrisoafi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kfgzlaoj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iojrajfb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qnrksenr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xsqdqoms.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2baodraal.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2chrlpcpo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nuxznmih.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mhnkgjjl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmkhwa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdbyrz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gpcgqonr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfwazyqr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hiaoboai.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2btspfoqi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pmcbrdza.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ttehopcu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llbdleis.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mrfzwxol.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhvkii.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eyhvjdrh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fehhzsvl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2eusnjwpw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2myftadms.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sjvtoalj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xpglspcl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xrxtwgov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwudlbbh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2djbnglih.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wldxiscv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2seonewds.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dztntjvp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2twmiumfl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mzhtomou.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iurcvevo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iatjiigs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ptixvkgj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iajxdwvr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kiqurujx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fsiujuza.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2haqkkchm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2unxhqxsk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uphvpzdv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aopkmstx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2itbnophe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ddfpohvv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fziqtvtf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kmkptazh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qbinnmjp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cvbuzfmn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ryqcxbwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqsfvjdj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gccdvlxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhxyjuyo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mgddfqpd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jrgkmueg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mjwzzlnb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpuatuih.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2chqyehtv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hgbllpgs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kpunjzxg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wmicbioe.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hlkufhre.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mkhoswao.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zksldypt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zklgmyaj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dgqtjxca.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jhpiimcx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fqtukamc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lnorxign.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ccetxzrr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qkqouuxs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2aijsekxc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2bpzudvak.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2raporvcx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qytaqmsi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hhdczrye.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vmahjsqy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jxtfpamy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gybrgrrb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2syldseki.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mvlclyny.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lytiweei.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cqegbufu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2sgzgafak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wvadajrv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2kjnfecof.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2syvxyaij.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2asakxwvr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pplnfrjf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nmpccnvc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfktoayd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ufavsneu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ubbebntb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2lzstpafd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eljsavos.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mhqupqhb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rxahqnje.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yqxmnitq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ozspgkzl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tumvwcch.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dpucweth.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2irpiatkk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kgblxlrf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2cafeoyzq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dmfqsocz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wvwswfnm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wbzbbuih.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2fkzvulpd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2lraosvum.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tlggobbq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dwawghhh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hohxjjfq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ejnjeovy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2gtosinia.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ilxwtafm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2bkgrrbmt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ionmmifq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ljppvvlw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ynpybgzm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dixkuvgi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hejvkajw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2scwgvexl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2pblvffbf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wuuuezri.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2vxiitgeq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kevzjvic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vuhcibjt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kgxyfxcz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2mereqyrr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hmrrmdqr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tpafrygt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jdoitdgy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ystoszwc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2aczkcwqc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2otrotdav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2otctfses.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxidedow.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2afzpnapj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2btlgvsdi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oehasggv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2impuwzrj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2rpqbvxrb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tddzojfq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gzceaptc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2atogzvqn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqfulwkk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2dkvvjzxj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tyoeblxi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ohfgemfq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2twzomzqp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ftsxeirm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pxzsdcqz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hwpuvqhs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jbsnfisw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jrsakdry.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2osacnbrs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ypldxuag.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hinegpzw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2orobzcqf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ulbzapsr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2utmxcliq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qdnoqnqa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zugzwnyz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wtctlbid.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nopehdax.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oyuhldyq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nydihaxc.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yixrgakz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2obxmzpko.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2kidsfobj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ofqrnldy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mhdghqzt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2asrekziy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xwixfuug.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gqzeorpb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2scoetwrn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rzlxacsb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ssybbgqm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zjlyrior.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2cipxkwbj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kgqlrcgg.html


<!-- 参考信息 -->