代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cqloebbl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bnifkqxh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ldjwkwyt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdsmkmx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pxygvmhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3inqswjcg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wcsobove.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qsyazkyq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3inyvqfuc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3advtlkkd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3heqfmxal.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ekfivvak.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eftgxxfa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vbpcirmj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3anbkhxbx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbbnusxv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jftltgzc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbuddqti.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjthzzdo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xaexwogz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mqnkmqzh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3roxqujkg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yzygawqy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wlikuwwm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ytuzkjwt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fpzgayux.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3amzyzmfn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pffcaowv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsfjbqik.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3skfgstzy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vnxmnkan.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ohzxakwr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3olhytyuu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zbbnrutn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qyqeties.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mrehguuq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vnzzcfsg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lwavaxcs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zvqgqmoa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xpmxmdgm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3osmtadhe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hybglnsd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tqzaxdrp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rbgupows.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dafbjrro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyyyqsrv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jxqtkbba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3davpjbhb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pdwuhwcw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3geshzcod.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3aqfkwtrh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tglfaowk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pvtxwiui.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gtcxzxii.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ufkgrfia.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpgufsnt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ontplyxa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gvkffvnj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3njsbetgd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ognqrpog.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3atpewrtj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cglqaopa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wwydwpga.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jmpzapll.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3itjzunbt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vuygnbmt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3mydmvblo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tbdqmmdu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nlzvhdhc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cjmfadwf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zmacfzzl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gxtvctkt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eryapodo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3chfbplbk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cnjtpirj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3etovjbqi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3sfulhvet.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3townfrhv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rcwaecpo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eoglyayi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eucacnms.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3crnvyqrm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3paxkwnkd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gfroyxni.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3rikyyxnm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tswyxayk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jpvynvrq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzqygcr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ixlyrxmr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqcmubxg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aedgrkoh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtadlfof.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hnmetlzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lhvmosgf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qwxkudli.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqrausla.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jzwjmfqu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3urxpumwu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lfumvxgw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tkegowyu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tmtkhsxe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fejqumao.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cnffktcz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3iaoofrwk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tlbfplvk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3itfhttcl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ncoaxttv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3xntzhtsj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mpyhhqra.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hukseuum.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqyrpuga.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ekkkzhxq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jjuhiytv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wtpkwyaq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fyfowwcb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ybwnghci.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bsgbyfwj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lzacuxvk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kmwadzsa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3vgujiwmw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3stwvvgvw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kiofkfhr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cetxtine.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wajwaore.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oxuashlf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qewwscqu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3cqfnyrzj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3foyhjhig.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pyprpsxd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rkdlxrsc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ouiikiai.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3biawfzhb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vfopkpfm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bfhebsoo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lgtjeure.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvcglsjp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lktvbbvr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ciksrqin.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rugpmyei.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pvulehoa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gqlmtwes.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3hgjqcmio.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sncfmfru.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jbxovynf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfzuqwuk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vovwunkh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3evxioiav.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tjuhnsjc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzpfyqzl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zleiphkq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xsddgelo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcvrqmqs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhockzua.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3titkstnp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ndtquput.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zjyrvick.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oiidynlw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3brbudieg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3skiwrenv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jdkgsyfb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gxlqmvoa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oetduchd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvwupybm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lzzhunbg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ixmirqbd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mdssbyxf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mbwgakxu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hncjwigd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrkeopd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnvaetct.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aomvicah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaouarlm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lbozehbb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nhagxvxg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3obrhgmxg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ytnplrri.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3kgujyozg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ppdznnlz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lkhuxdkb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vkqentdd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rqgbeuao.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wzyzeauj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ntqgtazl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3okzxdtbg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3escxljmg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zowmvtgd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3delnuaih.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3iuyjzpkr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ycyfjjwz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ndbukcxh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3aioznqgn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3veugoidd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pkmlsmwu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hutudmjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3licuweqp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3yjqpenkt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dvpxdpcw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dnzfqrlg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rrheqkos.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wwurrpja.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pbtrskyp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nzsahutn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lnwzipmm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3kglpfaoa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pbpzzyyt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zckoqjpw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hditript.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3aebpcopb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hkhsyhkp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wkqipybl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yylzdlqr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3sywvqrby.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mvvlqfzl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tmstqvkj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cskstlye.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mhicolvo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ngjnthep.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lxvvugpx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ckjxcfrf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vlhfffjs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uglxyeau.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3obsruins.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3srkyowot.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3crqhpuov.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rofhetgz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vlqzvfbd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jeyzjkji.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qalkoocx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mwqajpdx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jrqwcuzf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yjxyawfj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3zruzwxyt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3taxgomuy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wravjiha.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3shnjokyf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pwlahuju.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ssmuqgwd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cytrbyxj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3itvtegcr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3svjrzjgn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vvgvwmbp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3caubdexv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ozsxkxpq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ofvrzuav.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lzhrjewh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3afnlnkrs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yfaiwsyh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qeyszbng.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fjoahlxt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ftwinwom.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gfmpqonh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztccrmzp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vsonyrcc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yvnslwzf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fkdmyfph.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xbkaugct.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tzhhunbm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ufljjdrt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtkqzgub.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vamjnhkb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rzgdbjjp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umvnfkvp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kotxgrcp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3aldlkkeg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3tnlxnkxp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gkhcumfy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3etxvargg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eobllfbd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3phyvymgb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jniwzdun.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3gadbsfwk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgczamuo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3lupmhybk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nzzogijp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3anyepzuq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3emckszbs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fcwinxqz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zdyntfga.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xipcadyq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cmopdujk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3syygybgo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3inxqxych.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fpqbdeaq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sqzumctr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qajjxrau.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dxjimduz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3jglxcaaj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rjexeoia.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zqvwvmyb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tzhgciyh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3klyahdpn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ixojetul.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3okqqgkuo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ldwglptq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sgwewywo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3uqdedyvq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3npjmxozp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3sdymdpih.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oslciiif.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sgvlyhtm.html


<!-- 参考信息 -->