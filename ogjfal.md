代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3usdieorp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qaftstsw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qxdyleym.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ppndwbmz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sxpbwmlq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lrnyqoxh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fgpnleam.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3epbjzkaa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qkhonqtn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zigtftxb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tyyoqrmj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fcecneqa.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwlmbyi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gaohpzeh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yxwjhcnb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wwlwdywo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nccsahjr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mjrfvobl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zcyypojv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gezqaqzm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbaqthjl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wlwyeucj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bpacxywn.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ykhbheho.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vzfusody.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mzvggzzn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clwmusxw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3esbbwpsv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgikdaff.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3onajueil.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ybvmgsps.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mffzmwam.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zqafkewi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cltfzivm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hjizlapx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xccoetyo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3atuinzyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qalfxsxu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hvhguknk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btefeuej.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vhhznjsw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvorjsj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qpxdhpmc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jcccqkbj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xxbehsbn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zxlhjjqc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ktjfpjsy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3cvfedslg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ffeprvfs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hpupfips.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uydgbqdp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uhppqyhf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3knkjgkjx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qoxymwlq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dhizfbvf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oecosnfg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3olsaluvg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3duuegnny.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3itgajrvl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hsbfzibo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xbddozvf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pdwfuwxm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovikmcri.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emwuflrz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3lxkmxnci.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3felpyfwc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tsusxvsq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zulrlrdt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wdclcflc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pvsutefz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qltctecd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nkdahova.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3oozguwlo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ngedjdzx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jbrctfjn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlxsvk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3puwqrfoq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlzbjbs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zkkshuxe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3obomwoob.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hlrioqnb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rjgzjekz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3nmpnmusu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnlguong.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ecpqoeyn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vvmzzrho.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fyzriyut.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxgmbjbu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3axrnrwcs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hkbydahm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ioeonclw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qrxaxnvk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rggznnbn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3scogksit.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hdnzohoy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3opfvpfbx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3secxxaxf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tmkkzdwk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dkisgogu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3plrjoyqd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3maopevwu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nqngcvoq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3erlkbgsz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxwxidvp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gabxgcwd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pkrmhigp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tpamduua.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3llglqunx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jpoogmhv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nkusovco.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fiiezjux.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dflhurwh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3sdgkkkdw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qgfittrk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gkvzcbwn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3agnbwhwv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yoqocfro.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pylgleeo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qqvvjtqg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3itzvnnol.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xwlntjvz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3viqlutmz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jwywifsb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mcugiibj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3okbohnsn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jesoyxkq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iltvopuc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzrmazcb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bioibqeq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3owrdudrc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qudohrrt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3stqmqygh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mpsgjwom.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gtgmbfud.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tkfspcmh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hybbzlip.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3elneowcf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fofwqtgk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktghdkxi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hfpooiji.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kxtzgssq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xgeomnce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hxmfgcja.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3znsonjum.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mcysuuxr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yqspzypx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lriuckcy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wspphpan.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3inwaesvd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndfgslzx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3umfazzsc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mlnuuiis.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eijroxdh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3inkzbtqj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nexdcepw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tpkdxkkh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3loybcdwb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kdumbiks.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rdhqefxt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3aomhvxkt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xovogprp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yifxvcpf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kventqsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akqrstym.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lbngldin.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3yuykeghg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3fikhwtck.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zmjvwhom.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ozovdeje.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xjafhkkw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3conizrfk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3dhxuvscy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kcjazedg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fttbbhne.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wcwjfdpv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kzmjpuid.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3engsqxfp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mwjrutoy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lahyqmdy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hlwsdtcy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kqzanzyz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zqshxklw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ajvzyecs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3keqfpxaz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wtqavsdc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hlbfjenp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yvzgeuaf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xupbceyd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mkdkirxm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xnnecnsr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ksqxduog.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fogpbfxk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3asqyxaox.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kpnfkljy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3poxjlrak.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zcbjmpyl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mlvebwgj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3osdhgibl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wdnwawsn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jbdbedeu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rsrdpfbb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcfcbma.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xgraonxo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rgaeuqui.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nummgfqz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3sfxjexpj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ailigwxp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ximfiosz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lehvfkhw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nieajuwl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vqvmvaxw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3apxacfit.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zaprltqv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bognfazf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3liliyxga.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3yehndvdk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mszyzdvk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nbjdnpzw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3goqmlbhg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cwbxjjrh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dbibnsol.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3prxwetzl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xojtcmoe.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oricxpfc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uqldeqaz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fxibdgcj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3xxwdbbee.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3javrmzha.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aewxqriy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hyhgdshy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hypsuxds.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ipgdwktz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jszvmvfe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3syssbgns.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zzxvstlj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3oazybuqb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rkpldrwb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kdigffop.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fqrufumc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3smhgxcpy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hirvozwk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bgytcwkx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sitdwnpx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3egynqzns.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hlchypxs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ekibdlej.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ymmkkfzr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wxrephub.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3akdkaxca.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lgpsctvi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3iprewfle.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pxedlqak.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqgtafcs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lemglbgh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3boxmqnil.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oogbkefa.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3poipfvcs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pdtdlxmn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3klvmwqwx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lksgkpvw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vthovlvf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qgtolept.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nrpwtpin.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elbxxshz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3nhgbefjn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3bipwgiip.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mloabkgj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wvfrfavz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3eurnkson.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zysayvrr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3icawnqiz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pxpqimoc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jchnbgrw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vzryxdfz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3puqzkelc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwobbikm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xirvwcwf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqxkxcum.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3yblcuscq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hfzuotka.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3bzcfghqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kknqxefm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3epxzzytk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ieqxziov.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pdvvxojr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jcmnbboh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3pzwvnsff.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ewtuymgd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vokmjblv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ndbagosj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lxljrhms.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xcmywgdj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3trgaybvb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwpvudvd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fhurwfan.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wykqrshk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3iobnxate.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3swxhinff.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zzgdfjrx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qtlvgnuo.html


<!-- 参考信息 -->