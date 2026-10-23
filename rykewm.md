代发 wailian999

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3rfllnfuj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3phzolcpv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jcvxbrfi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ebmqtwdv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qftotgeu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3iliaalij.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rooqqadx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yfxypwyi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hthwgaqa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zhvkvxxd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bolylzgg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xtasrzxf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3twsjtpqx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3knlygebs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rrczkdxw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3vhvknufu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hsgcwvhw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3absdpjkt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jciyvlfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wjwnuxjx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bgngszms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujusjijc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxqazdxc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3nlkkknxx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3plxostij.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ufhjewah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wxviomjz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vpbgpklt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uppepvmh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mqyqaiwm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pleszmsl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rxlecvqe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpfowjke.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3aqhtvkib.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gsuxbfaj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gsdfznwq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pzpovzwm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yjptkdyl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wsneqdpt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gjvqzdgm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iyuotbgz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ddhdfhva.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nyihogdv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3polzjhmu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pveriouy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fcnygzne.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tuppsfgx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3patopjhj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aimkzmsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqfhtrxz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kqjoxsxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swkrvqvq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ximmgpbp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ybwbajmy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqtzjbdd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yvazkjdj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3efseqgld.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nwqbzmhu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mtzkwpkr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3miuqzcrq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3urtlwynt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hrmojzbk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uzofkpbh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmelpsn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qbebbdkk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jsukaqdz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3znpktrmr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zypwaiac.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcfgekbk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dnbzmumy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ubpvkzgd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3csovouxz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3klvjxwsx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gdpevdtg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3byraqdbp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnyumspn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fcysngak.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sddohaix.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kpfypkuc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bilonkoa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jzrzynka.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ycihwvjb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kgubragt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3myifqvmm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ssidotlc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gvlerpvk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ipjpmacp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3auqdshwj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iqqrkwpt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cixiuhlq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3cnbyaxdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3clyzfbqi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3suvpcuzw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zvmsebwu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mvywmzzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3luuzlqjb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3toyytymn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ixoxtbof.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uswwfzdl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zllnblpt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ewmptggf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rxrcwimq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dorippqp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3irrjrtjc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xddfrxen.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3joeoukuu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3clbypbjq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3gyhbflar.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhqkfb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3taoeymll.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bnzobifp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ychrbzjn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zkhhibed.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fodxmldt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wzmdkyxl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3viazztfo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bwlaklot.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ssnrukqw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3soxjjcbd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zjrzuruu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rispshtu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pteprvpp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3aoabgrzu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qesewmfy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3cjggklil.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ljtqvxmy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ktftqbib.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wgcoxopo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ymqkaxwv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rjebjgvo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xucblpme.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3aplphuhx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oyouihcv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ynsfbyri.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vddwggjw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lpgkibst.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tijxggbe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3esrmtqfe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gxgusnxu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3swfajzna.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3punfkmkq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pfnyaehl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gqbfqgal.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajkoyjyw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fkmzqsjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3atrxccgm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vzugqrbq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ltixiboi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbuwfjtn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pjixjhaf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhdojsgr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3frpvhmfd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyuzfxb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djjxhrct.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bnypxnth.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dsiwdaaw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjpcqsjr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vlumvvmk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qeupfycc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wqdejqyu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fggkktrw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ncuhntzj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3prvxiiim.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ptjxyyzv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fqmjnhsf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlhkqdnz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hawnbdom.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yagxrioh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ikxnmwvg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3uuuyfoey.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3aedhgeln.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zskqpzzh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sjvadxrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hofesggq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hattcmgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmwqccqx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3iuccryrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nsjbqcnt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vlbfwxbo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dvfksrvm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zomourqz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fiinrvvy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gnqamhva.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iqlbuuwj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ybajlxjm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nbepskig.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wgdalqbp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uwaczzlc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3irrejuig.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kqnuurqk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ekdidijc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wnpubzzj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mcjlkhur.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3haacbrqs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ginkcjkh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rvlnlarg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3stzvndxt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ticbbubm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccwzgyrn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3uxydpixe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ijagkwki.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lewsmldz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xcqknokw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrphcza.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qemohnid.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kwmuokzg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xgjdbago.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3aimiraja.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hypoaccw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hzkcmmbb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cgwqrlmr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wgoemysk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zsozareo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3anodaqoe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3fozhjhro.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nxbhnwel.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ifzlkhhs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tqcvoreo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zohmwgvx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ottgrrtv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3uikkqpvq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yxzzoace.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjqhxgna.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ddesnmvd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3krbytgge.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kkueozpx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3baybzjly.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kotjkroh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3nmemdjnf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cgzrtcxi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3brhakstt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3yjreghfq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3beyyljvo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3egoedorr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3krtyczqe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ziefjpbx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wxgnqwyi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dvruineb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qayljfpj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bcmtqhws.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3khanahmj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tdkontct.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ajbmofoo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3immshcdx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qfrltajh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zcdyjsay.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3txovhjes.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3beykrxzt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ntgdwljo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3txzueybe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zkfkhbgv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3fffeftek.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3oljwzfnn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mphlsmzj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wvzmbjvd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqmibmf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3sikskdbo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nsnvlhnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hneswcai.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gduxobcr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lshnljre.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uligdpsf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vuwnqnnh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3nmfzfuxv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ebyigxgh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kyogzkfy.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3larovats.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rryomefy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zfakmgrr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pgvigfgd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nbzgeqmf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rttbxkby.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zhoocohe.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wnmjoeep.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xjfqqkhy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldrvaykb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nysevteu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rpbhcpwb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pexyduwn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zzcbxdit.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wxhaavfh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ivqmjhbl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jmedogiq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xzshvvwx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hupqwsqv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3yjythigs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3povhrehp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3soonwlow.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iomunhcf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gafghhda.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3atvogdzd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tgqazwws.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhlcwzih.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lynjdkbo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wvuvqdsq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3clsctvxh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dyktcyom.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmppqcej.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wklufrby.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rwogshhv.html


<!-- 参考信息 -->