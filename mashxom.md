代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gsftitdcd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gpqkpjmuc.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gathigxlk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gybsrleiy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gwmmmlddv.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gtpszxwof.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gunnqmguh.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gmlujlivu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvkuwtrnl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gkspfhijb.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gfezqxdac.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/ggserbppt.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwuejeff.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gzyubmesj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gsbsiijdv.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gzithqixr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gwttumcko.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gpwscegxn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gzqgwzvzs.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gdnufmito.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/ghkidqigu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gchflatqn.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gbctdvqph.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gmpebwluz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gmpwqlnsg.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gluzjycnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/givnwrnrb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gcyzovnqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/godvjgtuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzacdvghr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gvkifimmg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goplnirek.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmpgibmei.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdwimrsbz.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gkheeknua.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gehrvriwl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gumhpahob.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gswbkfvvb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gougkxtln.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/getfoazfi.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gtazpnfql.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gimdylgwj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gmrwpjntp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gadrikzel.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghnrbemlp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gqkgawifs.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/grosgdhnb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gyslopkln.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gznqiwmgw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gsaslzdnn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/giywxfcbr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gwoeocblp.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gpzklkbcp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gsguunyry.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gttejpsgq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gjdkwacxo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gvvjrbvqs.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/glsoqamqo.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/giawxmymg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvynbjavb.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gsiymqjdi.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/ghwcrwkne.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/ghrksbwyg.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gflgagzhm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjbbidfld.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzusqxkpg.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gmtvylntb.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gzntzlvrl.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/ghjvukrmg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gghuvyzht.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gshfalfog.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/ggplfxbss.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gwimaohxm.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gvmfscnzy.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gzcrqpmcx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gywggniik.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gtfkvjlpk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gwdrozpqg.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gluewwtlt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/grppavuxi.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gpjhswpwh.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gqazhyije.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gsbrjnagi.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gkymflary.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gexpamdyf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gmdnjdvip.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gyjgdwfmp.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gomprjlpc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gcnregkgz.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gdyedyuju.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/ghoewagod.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gsfgqjgnz.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjndbuwil.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gsgcgstby.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/glcvbpxwd.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gwrttxcxc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gywgzzlzl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gdunuwabo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gusvtlvnq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gzaksludv.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gdzucmxxy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gwogdyboo.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gxqhtjnvk.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gjleokujk.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/guwbjbhkz.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gwcutjalr.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gasavtmow.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gnuxnvkjt.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxtzmjzyv.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gxuwxniqz.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gzmbdfxsm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gxrpjsuaz.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfbjlgjiw.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/guikqkzox.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gwtnvqzkl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/glcxcrypd.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjphawasl.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/ghdbglyzu.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gckekjftr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqczhrrrx.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gmccsbzpw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwhnpcfc.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gpaqiqssk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gsgqqleje.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gfymmdonl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkutmxtka.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gizlsybhw.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gjrwhhmxy.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gvxoqqsdq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/glexniofk.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gtjdqsizi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/getexhxhw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfeavszu.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gxrtrstrv.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnyncvodc.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gylusfxkg.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gygsvzamr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/giqtzdqaa.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gtmhfbnnw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gvlshebjw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcpwwlgod.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gqvbyangz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbgwqasje.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/ghdskwwhg.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gmrsmloka.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gwhspwflk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gokfvgtca.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gkvynrrcj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gbwgkpphp.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gsfqwvxez.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gldyboehx.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gbkiuagyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gpkvereik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmtwvqoco.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gsxszpsys.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfozfgcai.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gjofsxwyk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gttqpyurr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gpwajpdhn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/glznbugre.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gvzynaxah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gbgksdwjq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/grbmcjnwv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gdhjzwcef.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gwklmvzup.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/geevkbsms.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gxnpvikqg.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gwcjnuzob.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gyvprelle.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gimktaqgc.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gzouejwii.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gmxiknggz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gwkrhjbuy.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gpcysvyax.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gvzftelfa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gwveqxokd.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gjyyywehd.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gqstozvad.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gbiertdtc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/glocoensn.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gzmzhvdqz.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gycgxlhzm.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gxauxhbpv.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/geqecnikz.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/ghlkxmoma.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gknuhqefk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gvsnjxjjz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gjwmaffhr.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gflgitiad.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gabzetnxn.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gxncwtrzc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/guosbupas.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gapsanoql.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/grckhbqjw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gbcdvcdbq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gculsrojm.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gxklbshfi.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gcmlyuaiu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/grbgikbtu.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ggqxgomsb.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/ghrfjumnx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gepmqiquz.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/ggjmwfgpw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gugadrpon.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/glahharop.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gfpsspjgu.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gednbtsus.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gzmvtvnzw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gthvftlel.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gxkidbmhd.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gonvzjhxg.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gmkxqyhyq.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gfmmpdjox.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gkdamflix.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/ghsphisqv.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gxjgwzrcs.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gnmnojtdm.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gvnqvyccl.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gaxkuowrx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gqpymkvqn.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gfpckvfmi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gfgeqpurp.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/ghcsnyshw.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gzrhpofkt.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gtakuqztk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gvzczcsya.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/geiiqiaxx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gqajbrsuq.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/glnchgqad.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/ggsxxicto.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gzuitmlgi.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/guzibgmdj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gebdnpwpn.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gsnoenqai.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gedyvkhul.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gborwnytv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/guvmqrbzv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gnosngflz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gftlustnu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gmquvdnyz.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggubbwssz.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/ghafwhlme.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/goebyikoj.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gsmgbitgf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gnmkrilyn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnarwltio.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gvbywaygl.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gbgvdkvix.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/goqlvrbgc.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gpguqqibe.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/ghlfidvzs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfnsqmtg.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gsekgwvtg.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gamizosxw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gnhobfpmi.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gximlcqsw.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/ghgrnaiun.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/goylppfyh.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gwfmoxgcz.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjimdprbq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gdmyjsfvg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/ghxqxvrzg.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gyxigczue.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gsskatzxp.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gnqfpvdry.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gqxwgccbw.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gqezskboo.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmaynjsrs.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvygjbbnh.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqsgpohjb.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/ghmixnlzh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gwmflbfgo.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/glgfhivoz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gqyivgpvu.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gzdyrnftx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gorbabasi.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gdgxpmndx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gssnkplvw.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gnjjrwpom.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gygjxbstb.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gnqxvxxpg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gutbuqyjc.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gknsjcedb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/ghovkbxvr.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gznmpbrhi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsnczrixy.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/govbblmli.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gttgivyzm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gdnetmnsp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gyflffrim.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/ghtxyezsi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gkpzhkmsq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gqzlufxnb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gacazqdjx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gdoxkeccx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/glpgrkoct.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gvjkrfjir.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gjhtjdrhl.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gnryhlkyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gimqrfdub.sHtML


<!-- 参考信息 -->