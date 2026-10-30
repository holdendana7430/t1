代发 wailian999

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gsburvhdv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtxyjdiyi.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/guqafksfv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/glvozgxkq.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvddrgpup.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gzcmgmfwc.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gsfsmeuwe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/genzqeulu.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbcwbtsox.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/guujctoia.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/guiplpqcg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gvxvrwfku.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/grmtkkchc.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gymknybav.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gmskidgni.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/ghciftidb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvzuiliap.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/goqucysrn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gckpsgsgt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gpmwhtbrt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gxvlamtbl.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gfllczsrr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gfesdbpqr.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/grllacilm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/glfprjzpn.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gchzpipvj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gxaxtisik.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkqceyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gqembjiri.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gsqlavxlq.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvbpxqupi.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/guxwcqwzd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwxotxqas.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gzkwfyzfb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gpeqlklxg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/geyhciwcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gjfsrwyha.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnooystxu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gyljmcdgm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gycqxafsb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghgvohvsx.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcrbonaxv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gznmzxcle.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gwytimsou.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gfqkpwnzp.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/goknexlbt.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/glveovlxe.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gyvtxyior.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gwkqcpegg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gobapezhw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gmgfwfnjk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjdczkezg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqyvzkkwx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gbpvildcz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gmzpezfsa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/ggqtchdkk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gaynjlwcy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gihzkucwe.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/ggjofqgfc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gzcbacwbh.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gfxqgxivv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gqjxajbhp.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gmtjkcrrm.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gozxmqfcj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gvmklhmhi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gfvyouqtz.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gdvjclnyq.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gwvbigklz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gizllmmkt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gkhkvgcmq.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gbkndffhp.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gebohbzir.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/ggjthyhez.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gexxuevdy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gmswrphqy.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gbnwqbsso.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gdvfthtrw.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gqjrqgiwp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ggsncrrxg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gavpezmgq.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gqtlgicya.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gawymcmqe.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gvwzhxgyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gmcigozvy.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gryzdwvmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gntjqozri.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gxhbvphdf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbzxwnrqu.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/ghewnudpp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gznebukhp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gvyyftqqw.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gzyrtulen.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gffdpwsar.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gymndacku.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/ggztciwja.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ghmdqnpbh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/grashqipv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gmjdasmqm.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gjjatxwzh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gzaksixcs.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwhgogugy.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggefpnnio.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gijodxcof.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gyomxonox.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gcdhmkeur.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gvkhotbpf.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gdsfcljtn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwsxxzqlf.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gkkrtjvii.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/goijnqmcb.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gdsnwvtit.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gjphwztfe.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gozfwdqac.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/giwzpqtkz.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gzersvhhi.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ghjtlzmew.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjfwhwzpp.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gesltowae.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gigcwphtc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/grijtkyjj.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gybvcftfz.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gzstthrxs.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gsuoxgmdz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/ggwqcqlei.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grxfrclvb.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gxrkildyu.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ghstconwf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/giyhgmxwz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gmdzftwfs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gxjeacgty.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gdkfytupw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gyxutrpih.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gwgrqoskl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gegoehezh.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gjvtmcupr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/giyynuntv.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gvvhjmnqe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gmawxvuzf.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/golziyugl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gptptgjko.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/ghmwryqes.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gglkrafxl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gsndzmwvu.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gkeemaqzb.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gomrjedlv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmkjbwghn.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gpdwylofo.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/ggctvshae.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gkcdylxmb.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gtcwennjl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gokdpamhf.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gzjxwhgae.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gyzuxuiav.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gebgjkzph.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gcrlljkqg.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gdcirywag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gmzucdrmj.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gzzdkegel.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gvmotnafh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gwolpvnvv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfhkomlt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyarjpmim.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gdsximgcs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gftuumamz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmpxwus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/ginvgsylo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gblcwrsai.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggvvsaxoi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gdcijbicx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/ggzzvmsee.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gxnujnzys.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gvtrhzgpf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gmixtbyyl.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsdhuieav.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gysgqeute.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gzqfelnsh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/ggoznktng.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gnpfvkamt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gjbqpvuoq.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gvmwuyfla.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gngvtyogm.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gnzgdratd.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gsbcgspjk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gvhlwvabz.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gcgtkdjmf.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gafvmwwgj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gfplopjjl.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gpirylswq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gysujomsy.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gfoqrxsgf.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/grvnaatvk.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gvavhvzrd.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gfeqyjplg.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gtevdathz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gsgxwgujj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqzxmorfv.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gqcggaast.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/ghlmdwjxh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gxeuqwvgv.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gjnyggdbt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/glcpvcrus.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gbtammvrx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gffjutlhk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gfzlxnzyp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gcyjzqwai.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gyfwrflqo.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gcbghsblh.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gfrjlijma.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gtwtjkjal.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gsaoyqhmi.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/guyzsotvt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gvlvxkmgk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gijkysrjt.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gucnqligo.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gvvpevpse.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gjyinkwfr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gpotampzw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gmtyytcca.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gvwadwwrh.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gqpezzzmv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gmscnnqbi.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/glzinunzk.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gggzqeyqc.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/glctohhsm.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gzskclmbr.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gbsfhipvc.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gjduzgomo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gkuecnvjn.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gnwzewheo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gclbrvjct.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gnwzexhyz.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gqutdhdog.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gxpofisdr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gzzzdtrjs.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzvwcthot.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/giukmfekw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/galiwkito.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/guwfwgqgd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gtnpyfigp.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gthxusapn.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/guxulyikc.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gghoxjhkq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/geyaeeljh.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/goakwtfja.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gmetifffb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/ggneyelis.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/girzsrpbh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gofmoaile.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gayzjwhcs.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/goqgcorgx.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gwtrrchfi.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gymztaztc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtffugjca.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gncxmnnih.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gmzcvicpu.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gpesksncy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gfkvqvdex.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/glradnxdj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghkpxrnvb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gtrhkbfsl.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gmmdhuref.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gvrjfdcsh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gpjbdwjqk.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gegvevcxs.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gqcyflfkj.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gzeczvxqb.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/ganuhennl.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gugxxplmr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gkvdqlcys.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/ghsamlmzu.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gotamuyny.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gtiwjhbpr.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/grwrunqyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gyaidlaee.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gzibdoxut.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gffjaxjbn.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpiigpnza.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gotfetoom.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/ggepwrzux.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gvzckfotr.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gjntbhykb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gdunhdgfg.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gwxnqzsfq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gjvlpbhkn.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gxrwqzuam.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gqeebpdnd.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gizilxvha.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gzajesmws.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gftbpycuu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gfbbglnsq.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/grcumzjzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gpmecawpc.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gbzaoiili.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxllowatx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gdzjzlmgg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gflytvybm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gumlzqozf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gyfnjkejc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gvctbzqqy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gmomcftab.sHtML


<!-- 参考信息 -->