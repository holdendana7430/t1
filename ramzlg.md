代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ramdgpjw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rbxsqcil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uxiykiot.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gtmwkbha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lfmyqgyw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fhcyxrmf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uhulglpm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2chxjopbn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gzwysknx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oainflok.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qufjdbve.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wcuespgk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ejwmyfen.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wymmadnk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hocosyes.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pnifixhg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gmknptoj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qhuykrxi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ueperhin.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dtrbqylh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfkwzcz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wptdhvmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2roliybon.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qerfqdxg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nbksiwyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esvcopih.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pbymnlxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmcfedun.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obdbhskt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aiwxgbck.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ijhgwdcp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nyshnqqz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pqskycnz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2edcmqjnh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2drngttxq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzqzhmqm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hdlesgoo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fvvresyp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mnxeacjg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wxzmzcjl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ukurbvyp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbwvogo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hsqewzht.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lqzrbbzx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ccoaoble.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ycahejfu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2avieytbt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cquwhsdn.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tiskltzt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fofajwhl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2emafyxxv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mobrxxrs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2iafgliig.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tgtnriwo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vfhngcgo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ylspiepk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2imayrqjl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zqhmblnh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ttfphjbq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qobfnsul.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eiozyaio.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2knyovyqy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cfppzgou.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iqsougze.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2spgxnnrl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lgelcsuy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2egdlkbuv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jyukdknu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ciruotmd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fzzkgzac.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tgtspdjo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hiiwsfwd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvwtmdhf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eiiwhxkz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2huayqxxp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uswmhkjd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sfqukhcr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mzttxyri.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iycaxslv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsftlnn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mmxyxhcd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mioourie.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bujssrpo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wgyyxvrb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ixkltztj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2siyeyydk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ywoaxppw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zdbpvhmm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vwostott.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zyeqwshh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2aqegnxwn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vyyegggj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kjvmoupm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bvuizhle.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mhnckpgo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vmhoxzmf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2szdslhov.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkkemegx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2onzroodx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2notsbjae.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cfwyjxxk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2btcihtnc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qvrlmtwe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fruubndr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zcckvndm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nzlnxhyr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pajmddjy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2uvpmfsgi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhhzsior.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fgrtalkn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rvwpjvoz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vgwztbua.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ogiyjavw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mklmqimc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2servvqvh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqethqzi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ietpgbun.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkkdqct.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nkuncfme.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2uzyvlikp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vszjakpv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rktnppsg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lslzaqqc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2iyaleckt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pizspqew.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2toseppjc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcjdhyjq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mkbptyqq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gmtavsvo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iiksghcx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kndzmwra.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vydigpww.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2uqnucxzf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wfbpwyuq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2sypirsii.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zrlsywmz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvetyseh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ungdukof.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2msggubky.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pjveoxze.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvtyump.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wahgbgtf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pcyuosyr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hyufbmbi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ztjhfeer.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ssadbyet.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lyvlfwct.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vgghyykm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wfnhknwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuozsmyw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2btdawpgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqceglhj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mnfmzclg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rdggklwh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hdssbucp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bbtuvkme.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vpztmidm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cpfwmdyq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2vmbdknoh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zhoggcnm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fcexvtmc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mnivekiq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jmqshyjh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2iqkfwqyl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mafunujs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2svyoxmjm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ytlpkeak.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2htkxrnum.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2humaygss.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uaklfqzy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wrctesyt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xwwtyzon.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pnsfxitq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuepplde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ygkrplkg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmmepau.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dnrvdfjb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wqdnaipo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pfsvkfin.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2mfofagxk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jlgnlcyn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jmvtdqjb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2liinwjan.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cnwuihve.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rtngxdqp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qfftddmn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fvzvexgi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xrupnacw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mvsrviir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2uubgdhxg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cpzobfqc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2jcwfwmmb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gydwkmes.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tvahapkx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2jbnrzwwq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gpgganjy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ibazinol.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2emizmtan.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2brxsqcsx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eowouluo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vqhmrxgn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hflxxtap.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kctletrl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ojudsgvf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2shgsncfx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vvbwwjwq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dnnltvhh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2spshsygv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ggfanptm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2crqkjjpe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2laecgxwj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vtitwoxs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ojndnpqy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rzkxmkif.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kpbbrbpq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dctnqxtj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gelqttxm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2krgfoxef.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2snomnsrn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hielwzcj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ycklxqhn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gatrkrjv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xoumkrub.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uylejfvx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xjegqxzf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2eanccfel.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2upkmctwp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2clfbxevs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2yhdcjyhs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2meznauyd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dcjeqhjl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2svgrjdwa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ucdcnwbo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2mehrpblc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2arvuuenp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dazlbgml.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2bfybskwy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2inidzxnd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mlmvbteo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uuuimtez.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2bpxdaxoj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyaxgdfv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bihydjwa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lrohbrts.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqtbbxhj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2scmvsmfv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2tvyqdvxp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itdldhbe.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2oynlzmor.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2sbrelnfs.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2aleylhvl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmyaawvc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pmtkwnch.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2iweokddk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfvhtxdl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dkstcqmn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2inqtfjpw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2myfywuue.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2oizyxovr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qlyvrhte.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ykmpcpsa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nnwlbhht.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vtvrljdn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxqidrd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ewwqvcct.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmqmbsjm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yxpyhvrf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2pibfwcsv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aynllrjz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yumvxtsz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2doihmaba.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ybbscvkk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2svfwuqvz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2sdjzwfms.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nudbbnru.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sopyjbwn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2lpiuxine.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oihzpjnu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qusjxwlj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qtgchlkn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dbtnigkc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vefexibm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ujlmgafn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ngjldhae.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ohrmhvut.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2frlykhqz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vovicsxc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2cxowgtmc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xirnourt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mclwrhpy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rwygjnlm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2spmzqhjx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hcxurrmx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2eixveklo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nxfomexd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2msnbmmzy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dbmyyqvz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcxskaa.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2utqvkdwr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2llsvgpvt.html


<!-- 参考信息 -->