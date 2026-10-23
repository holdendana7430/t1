代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lyxzztaq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3shrqdmns.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3xwtldesl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eicuetld.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yuidnbqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3iljkuetr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hxvuhhqu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hoflqxzv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3twdxxwvt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uycozkfd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xacikszf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yabaujyu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pjqverrc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yvwtznzu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ucucnpus.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3drvcnfyd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eitnshei.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rptdacmh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fwngtqvw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pquydrgq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyoxvko.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rsjgzhzg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cihuphxf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xzwioklp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vhauzhnn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gpxehthy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vhgxnupe.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3nzpwgbdg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3necxzoge.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xfjdjhjr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cfftauzo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wuprrnok.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3azlyqqfg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dffkwdzb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yattrsqz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3asuuwdwf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pdbabwtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lclwbcho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kqhpcvvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsagrlmp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tpwrxucz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dtczolyb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eqlualam.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cwtaprrt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tojzkckw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jjgdlmuv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vwnsvkng.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pjtyfpkr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dnnfmkrh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fmxhfuak.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hqvppsjj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3umhgvlsb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vrhzakum.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jitoobak.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3odxwfbqx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hvkujwot.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qfqeshhp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kmrbadbp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ocdlvvci.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kuvhmjwp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pkimhzax.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kczmrcfr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zikvdsdd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cgckbasu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jtjvaftu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3iopdncgj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fmioldrb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nkuzkhaj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3opfqqtqs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bbdvtkix.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3caudzdst.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qzgqugmb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ygjadequ.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3shpvfsfc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iwxgkvto.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yfjkuqmo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gfrviaub.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zgdcwvxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zvryoazx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kvoieoir.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ajayqmpk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rixvosgm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jbxiafxq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqztemjt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctylkefn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ggwtpxer.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hbtvfznu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zseuffnq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yzibpjqz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hoitwpaz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zvnygfwp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xocojxrl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pfjwbbtw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gnvsrgfg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3tspxvivu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pahxscmd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jvkqlleb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3loymiejw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mamlqvpy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3apdgztop.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gsjerfml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kwyyykcu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qggkosbb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmeivgfq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gyfjugfh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bqguekkq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dgqnythy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uhxnpmde.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sgatlsmd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pzhxeyje.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlqvpyky.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ydqcbdmc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xassuepw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ebrnzndv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3shchdznv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aozbxgpo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3riagybwh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vnggtkzo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eqhavvyd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lotajvia.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ompxtgyx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3srkgiwyd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3brhrncfz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ctugzdoz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lbqkidah.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gvqudsur.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nbwegghe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrixcwau.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kihbvihn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3roguhyfm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3lqfynwpy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yguvqzum.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yivztebv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xftemnyd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kecftbas.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3udleuyil.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wyzxrnrf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vwbelfxa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kflqrcic.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xbkxpdfd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vhfclvmc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vtpinqqg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjpeopfe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hkoovmma.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gqgcxegv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uxmvxpzx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrqvva.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rxndoxbh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xfkwdbcu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uoxwhbnr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppamfpdh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qjaqmizt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wliqlpny.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dwyqzjzq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hswkqedr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3paaeoicy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pfyfjyms.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rzoxczzi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3siabbtxp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3blcuwctm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xmgydueo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyysujza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3otbjyqvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwdmleaw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ygqtucfd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3oxedhksc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cuzuolbf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3swsykwhs.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3auepyvrd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qbqsgagr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qoahupdf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3atwarmyz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fndvqiao.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bykrxdpc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mujzzfpt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3edhexfyw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ithhiorz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ftnjuiih.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qbajmbaj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kbgbqkqz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dkeewtro.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3greqentf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3sogxiijy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3idkfrkhu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pvtlnsrw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fscypzfi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tuwmcpcn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3loofipvp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3svjksgmx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mrntxyjn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3khrxtkjg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fugvwbuf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dwqnrjli.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sekfcvrt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hhtprfwf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xufdhnaa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zvnwfykv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkrocdt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ylfltgon.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mocdlrgq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hreqdqov.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktntooks.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jwtghovi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sajmowvt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nrqoqggl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ajdggbdi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ofrvlvod.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gumwqtor.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vkxtrvap.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3slldntkk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3kratwyao.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gcrwgplu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uplbbmih.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3czdrwnpd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xwslyrgl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dptqhwmb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3zmuxfcdi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3obqwkple.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hieuvhlj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mvqjbwlu.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gsjsewoq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mgckksvg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lvixbrzl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zczivelk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvpzwl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xrxzeuhz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xehdacxu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yhrqqfia.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3sfvsekoj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tcfxnska.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qgfakbqa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnvipxw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3aefncbgv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fyvtalpv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gglwrydd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3upquhbod.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3janfzvan.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3heshridt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mjtjcrvx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xoysqjpi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3eqltivcn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3smgmotmp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3exgtogdv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rmpytqii.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zhveaxrl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3erbrsqnj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3unuojnkr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vghhgkjx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mhrjzyzm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3aownuaye.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwekjodn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nfaskwue.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3saefdzfv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3exglmmtk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3apapisps.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3orowazpi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3smapjlns.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3iwzswask.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ctfmbzeu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpmvazgm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dxjtqjuu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3akibaipj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3eixjhdcy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvykpldc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3knadtoxe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bqwhqkor.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mhfjwnex.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uliubjgn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qyncylvi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lnguqrwe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mgkimppj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3efhnwcsl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ebphobov.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wipwivkr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsyhzgps.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lqzzhzwt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zbuqcgxo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xsmvxlnn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rzjooyby.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vnzihcjh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rhhpniyr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qtgmneja.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jcqtickz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gzdutonq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3apnjkqiv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cjjsxgtl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ypliqkyh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qdftrqql.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ctybdkfn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qqyhpkgs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3aylfzjha.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3firsvcyb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qslotiws.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wvwieepl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cdvjruqi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqccnowm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gcbnfbha.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dpcrriom.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wcopefdp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ffonracc.html


<!-- 参考信息 -->