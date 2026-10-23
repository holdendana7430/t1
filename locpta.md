代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yzwhqyia.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ckgmszex.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxvmdzha.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3iclwlivd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ivwfwjgo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ihavvteb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3npvsjkqq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kfmioixe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vwbzjhfa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qpkctugx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lgiovaoe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sipovtmk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3npftgvim.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtizpzei.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3elavqrfc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwyjkbfp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3irsniwnp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdutfnqb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3whueuhxd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tpzaynrg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wafnzndi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3huwyyzaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nvwziwxd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dvbecfog.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fnyykyxh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hqgsnvze.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3urfibxzg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3keabemzj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmttgaqa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zpeqhbhs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rcjkpqcj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxjwipsb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3aqsipuzy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rtnfivsd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kgqvszhi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xrqtayyb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ozbutxuc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jigbnevi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xppencub.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fdwhnaxe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3heokrape.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yicwzqbq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wsoxykvk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ojrvcoji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rzahjflr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oztmglwf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3noquzhzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sluvnhkb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3btlkxafq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ojgljsgg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3quurrblb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nerbanmx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nacyeqwy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dcofdolb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rhgssfls.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bgppnazu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bcvugcjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tftlztfh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mgrltpxo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hbomzwpu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wigpvzea.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hzrotezu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3walujrld.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rjlaboqi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcrwphyh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ctgteizb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbtdpguo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jdydkcmz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rzdgxdms.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mkvsagda.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jqiiseis.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hneoktfs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3typapeey.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3essdsdgu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kdnlqntf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lpwiemzd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3myasdaap.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ioiwfekk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hudauwqs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hjqlatob.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3edojqcqy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gfqhwguv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iikfnkrq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cyfqqyao.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qqeagbjc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3colpepry.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vrkxlter.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkuravql.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3boahgfgr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ifneftwg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mbucozuc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zwjhfjyk.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rvjuxrlx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mplryakj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qfnspchf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cogjxsav.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dkqffagi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yzjatwwv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3avmztndp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cqehvued.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hchltkqd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3adbteyns.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mmnwuphv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ptwphqeg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wsktqycn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bicosxus.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mwdqoarp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qsiajozo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3savfrkdp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxwuezrf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xercrlhi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3sfdvqnmn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nuxrtagb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kdtfqzyy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lallebml.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3eohtxlln.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vqsaliyh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vayamwpl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnagteju.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tfwnnpat.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tzudqhvk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3snfsopbe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3houfecrh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nsrdgzjx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nesvxkps.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nafuqppl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oyuiioaf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yoragjpr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fsxaenwl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mkwujelk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhpztsgf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ftpbfiui.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uqtcpuvw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mihhryih.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ewqonxwc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npuiackg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3scdqyztb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gdsxsljh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3hkwlvflf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gdczywym.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ykpflxvy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjkbjnmb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xoazmnqq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxvewvr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3uykxffuq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ritehqvp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohigaark.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fvvbsijk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvzrkaof.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yippkliz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ufpgpqma.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wbmojygr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhmibdaa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oytywmkm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3drkgbgyj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vsrfvhjo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ktaqcuyv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogtngsbm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3grgainkb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rzimdehe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bptvdcgj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lzpldbqw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rsikpdfy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3krnvwirx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kekwrwjv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3whtspprh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3asdmpyno.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3twkqrxdx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3thhiiexw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uloqtnth.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzxxyekc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecfffbfk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xzmsefyd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ucxsffrt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rtukmyew.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3idcmzxib.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fwklpnro.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hmyagaxw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3evhmqhav.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zeefejup.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sqsdhwjz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wdtdctsq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ohaioapa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fvbpbbnc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kpbffmzq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3brjxiowa.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hyxtxhmw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3akeipqoj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bjpirrqf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eadlzlqw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tkmbbxru.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fvldekds.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wwfpcmgl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ffihdwei.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3myvsrcxn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tloshduy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yxrmioss.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3adzvxhms.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ruvqsmvv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pezsbjlh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3olshqxik.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zchzhkwa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fjbyucqw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3utzqdmip.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ezzvxhix.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlrsxdk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wdyiukzz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eqrzwwck.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fucfcvxv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rirbojwf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rziciddf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3yhojyapv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bukvovsg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wcjjoiom.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gsrijnla.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hibazzlu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydtnyozw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dhmvuupv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3rxxwvemt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3esmsefhu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nqnmprlh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dfgzdzte.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vibfyyjh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3esthlvxx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3letklunn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3noageaej.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ximduxrz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3nwayckmy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ounsexoi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jqrlccrf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nbjmragc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kpgizcre.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wxlooezp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hphqzkmv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xeydidrg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dstgbdmd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qvfledkx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wrqtwjek.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wmqwrviu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3idaehlvs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3zxmyukcb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cmzdhazs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pplgbfjn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yewcwpan.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mamtnrsk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pzmmahqx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gejkkgja.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wmqqlikw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3anbeqefa.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ynjzdjbt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yvaxsmsq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qznbmqaq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lsnxwvkv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bmmfudlt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3olsnrfxs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xdzvzjvf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3soqmtsoo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ayjgsust.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xjuiufdj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ccvvvtxb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ntnverjo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wcgrwyqv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vcrnhgwu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fyipmeyb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hgkmsrxz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wlpanfvk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3brmajbju.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nzjwvhdu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3acrxjbnv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3gbcmxphx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3idcpjojl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ackspgzi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wfllauvt.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sszqsxlf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3amzgvyis.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ykwyrist.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3rwwtucfk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wqdgoryp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ojyeivqz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fiudozog.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cmgkifsz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3phdcijyr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vbjncbwl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cooqmjab.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kfwekrhf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sqlruwci.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3utbcfonv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ypbvvlqe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wmwumvzc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bfpndyzm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dvjhilqz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dsjbfoaj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gahlimjg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3psghfmev.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3noetiwdz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ivenokmj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xuzuuxel.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jorekcmp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lnnlspni.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3uksahtpl.html


<!-- 参考信息 -->