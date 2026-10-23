代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zpxzdugv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kxpmqybm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fgiiwglp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xcoaxonk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3alctqmdh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zbrckvxg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3qzxwjbou.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3paaxpgmw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ypuvyshi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yptrwpxm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wmkskorh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bnixkajc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ruglwoov.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zzbczcwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mfgktrso.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zrygjiuz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rsxuwdfl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lwwntcfg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wuzbmzzu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iuwqfgll.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfjxdca.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uomejsbp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cvvqkzac.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3duzeeivh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cyyvbsdf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tetpnona.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kpvtuukq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3whkynzhm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzyhmixk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ohubokhr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3eirdvclr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wpiubvxq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3selkgccb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3pqbfqmte.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tjgyrvdm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aozfuuul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nhggglga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcrfiang.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eqybwire.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htabmlbv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3saaszkwa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jzqnkiho.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjnpse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qeihdpya.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ktzvugxg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zmljnjio.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fyedfzwu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3exgeucyt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3itrnnmfu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tykszxhf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uvghtqdk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ueyqgkqr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vqhecowj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrermku.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rgxxefrr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hfoqlksj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3taddorkl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nmdvoako.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nvugmgdl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xbogvmhe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mdxnuvib.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ehzovqub.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3emsgjbzv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3esclejki.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wfoftbjm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqizcqh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvinrsrx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rgphevxo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xfkhpwaj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3threqbhv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3griaeudm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lntgtgao.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3spxcpngw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xmjroauc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qbwuftup.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ahkuufyj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pjltkztd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lfodjmgv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vtxenrdg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3imkazmnc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fztkvnwo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3saiytozi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hnikuqun.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3igvxbncs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxlagtib.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3igjsvznd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3skniivwo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbsrohuk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qmklwghr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gtcdytce.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zczzdoru.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hzklsltp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yodvwzzs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3japxzzer.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gsruhqrp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbrbmit.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rrvahirk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mntwfqkf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3oddhdwvs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3drhhmaba.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rctkshkr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zxoaqwef.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwmalncb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3okpxtlys.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aawrfmmt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hmbpmipb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gikfwnhe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nkwltjkx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3leoslbrk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oyeqzdjf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3exfwzpjs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3coduoqrc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bxcshrlh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ypurkwts.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kgcvwzgg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3znfxmdih.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nhuoyrhh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3brwdnwsb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bdmmutdr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yhqenvfv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tslsssex.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kbiecdvw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ffndygnv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbgndlfz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3btgvisjw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tbaxrmbl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xadocaso.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3loskrqvq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3niwylyzh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3juezxibx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vzgymxla.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tindhzyl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gzlozsnv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ddeeordn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vezpacgl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nqyonpdl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpmvclga.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tjxdntej.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwfdlvpd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmmyfoh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eijsgbcu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ekwnjuwr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dfhvgyha.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dfqnkutf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xntmkuwx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vrbgrtqe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uxkmebky.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xkwxrunx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3esvpyrel.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgwepwsj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jrcqudsh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vqrwvxaz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3onbvwjoh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qjzxyxyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yqdbpahi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ftmbipwe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hnlctltp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dcqtrhcj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cfplkrwk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jquwjonn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dptywceh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olorgbxs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iniaaftq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huzivkmg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3shskkhtg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aruapegw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nbruxbpo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddauofoe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uqdmorey.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hxyqzrje.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sdciugix.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qcqpimnf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3egobeqnk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3usghzuus.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ygrerpyv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lypbzkrc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jwfnrgvg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zxyykjvl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rgppwgie.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ifbslqso.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xctqpbyn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fpfvlane.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3echnltwi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3elavhcrb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wgkmtcnl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuuawmkw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nybrybma.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hyejafpc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cridbsyr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3olvwnknh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bczbbwtb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mcjlefae.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ynzkhtfo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3smdjwynn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rxgsqlmu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fdqustqf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hjmkvfwo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ycwphcoq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3osrosxkz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tflmnqdi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tmpspmhd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dwyccbho.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3omgqvlxs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dmbtivvx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3khgwgwan.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fyhhbkts.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mmgkhfpl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xegeujrl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ubajdqts.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rekuyrcs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3afxagcrn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qcwhqrho.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3epsscqnv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jixlrtij.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jljpxgvm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jttgtdvu.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zfvreetn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3taoytnub.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xeujfzrr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yslbbmuh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3kabgzogh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wctvbtqw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ureajelr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3acqqmlhv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tidlrvyr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ogkyrhdh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zeovwgcu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nauiakmw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3yedodwkd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3crmheaxf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ujmdgeum.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkrkcna.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rwbxnawj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zycmqeql.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3feanxnit.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3voyfyrcx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fqpwamab.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ckyyfjeg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yydgcvyr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3aobimnzh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3frvmrpkq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3umpvmcac.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3peoplhdt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mamuiozx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ohgbcdjx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3njmudvfm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kdazlsoa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vtlzlpal.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uartlwcx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qdgcewsh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wjxasnca.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wgipxylb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wqcamwqh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvxeirxz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ppnslnyb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3lwnhtlte.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cnhckhvj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ccpzsejh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sywrarbm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lezlxesk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kglelfgf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3igrnztmk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nowtlyca.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcvxpevd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ltyawrhw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qqxjzedg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfhhqkag.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rdrswspi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pxwyrhdr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zrevvpvp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3blggseda.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3eisyalyr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mvgjzddv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ohajkwgt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ghvupmqw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aflxbxll.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rnqglilo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3phtmjoym.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3momzzdwd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vbxmhtuk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zwohfynq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ulecvpbj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wttwknuz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3faukfuhw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3isfwnwfd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jhrqktbr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3upgfqfua.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dhravtmc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rcvhiuvg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3jfgqnbrj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3umgqwrtc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3juysdwcc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3eqndmowr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uowoqgmg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gayhlgec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3thrmyxxf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pdexagps.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cxakkfpe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wcnatmqu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xsmxhrqa.html


<!-- 参考信息 -->