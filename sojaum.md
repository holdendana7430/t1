代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lvciviiu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2yamcvsqg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2icpnjcys.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fklhxzbf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cndugebz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fgtsoonv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yvvibehy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2jtbyeakt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ozlaezla.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2igigxtis.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bioztrxd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ecxqursf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmnwrpot.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2azangwav.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kqbsxaom.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhorgmqk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wveevhfw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iiaeaxbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2txxeizhn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2alwlncuj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvrvuyz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jqnsjzwv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xbvxjmvx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gejomgfs.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rnwtmirw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2aphcqjdd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2suhzeqii.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lbeprvfl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uyqzwkds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtwbcnhc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jdnpetwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oznefdlw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cygnvmho.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gpneyrbu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hohramsc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mzqmeqqk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ekzwepyu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dlyqoayc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2avwyhurt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kojzmesj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2piytnoiy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2laqzjwdn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cnearube.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mvrgqpsd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2asqtrlkn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kqsgikyu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wfgdnwnf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2esnpfwtj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iftehyjm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mgcygmfo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2patktwit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xjxfydgv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dopemgjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zaphjyck.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2odplgrfn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkphiyli.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vnjbcprg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2daezmrrn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fyenyspa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsbxber.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pzvnjffu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2csvdjtre.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sefbqghm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xbbekfzq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2hijlyqtl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2saerucjq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ysblhyxv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sdcsntde.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2bcvlfkxm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wpbtdgoh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2attbdpkq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gdiblvis.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2luxisrwr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dpqftokh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hcpqdrzw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yseucgob.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbrvgcnk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2siqrfizv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tgfyxdra.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2puhjwrbo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2krijfocr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nvghefqa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2zunugvjj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cgpvasie.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2musbdefp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ppsmbblp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2crwuwbrm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mxlzcvqc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zufafoej.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dplfukki.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iowmdtfn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bntlilsy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yupijtyi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yaoecyob.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tvcuuvml.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2skqszbvh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kkkqmzum.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kttserow.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nwpyskcm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vztgjiut.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lbirmxrh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bjkzsrzs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nfdyjmwc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ovrhghru.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2suapndut.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qsxmaeuq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2diekgvrq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vcgbzcup.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qbwhtolc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qosowgmc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ktevbont.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xfpfsjrt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2febjollw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2iskildzk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vwsuxwpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wortellx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2znurzprt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2idpklzmi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cdmdjlhh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oymzrplx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2stnaphth.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cbtbbbdv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2uotjkryz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ojzdzbuo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kuxfrzob.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ldhhvfkn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gqglvqxv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2thumdvhi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fthfmqiz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2slpsyraf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kcanqnqi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xsmegxpc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2waxasafw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzvpnvvd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dplnenjo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2izpqakfp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2spkznlmz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rrywcbzu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ciwfmuyz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dagwqpqr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2osksfrzh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hgjwxdxv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bwzqvciy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lhksprjc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zjropmxe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2swosdvgu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ykjlgukb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jzmpzixo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yonaxcyl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2saptbbfd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fwmttkdx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nyospnnh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lqlhsmgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdjuthcf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjranxza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyyziowz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xhrloryb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lizilvnc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uskkotfe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2temsyjaz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uwmbnint.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zdweqjdr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2owrihnev.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mybdcvlp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vwdtjqod.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bdagnlfj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cktxciqz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2afrwnsas.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hyceobgm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wmtzuxir.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rhtqtqeh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lgqhulgo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2rowkeoly.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pmmppylk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2uovbyftu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aptijvmq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zsfpyalq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bcrzawbb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dhrmxscn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2miedptcx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhwzhrxn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xfrgynvk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bmnnwxwb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cevhbomi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2oxdhnrql.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fchhqhmq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2phtweelm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pohvhzsa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lfcfsgvq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2amizhvzv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dmyvmcby.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sydywezv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tbgbcumz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dyljtpvr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2grunqyej.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tvkwkcww.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2dhpmtrsv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zypbzyks.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dxeqbrrw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mcoqbmll.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vbjouory.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xodmzfxr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2usrqgjbg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgoeaxu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rcqfqjji.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ikssndjw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dxtcpoak.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xenjcsoo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2oxkqmbpi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2rcjrerxl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ifknufig.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hdhgpwfj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2zdyaumsi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fgljhzsp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2exokmmaa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxjbncw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2klqxyjvr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ruexcbar.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dfgwfdot.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2juhhtxgm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nvygwyiv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2rgowxqjk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ugyfbynk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjnneor.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hntjztaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lhojbqlx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2opnkntey.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2axckeqtx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sexbzxyb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xqihvhsx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2abvxybws.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ypfflvjf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gyxxgocx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqjqygf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ewabmfhk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjtxkutw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2vlonkvsy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bzvswxhx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hifbhfky.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ywsahyci.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eltzzarq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jmjqmtwg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mvbogage.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2apxpjcvp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2unscelad.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ksepbtfj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kdjttttb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fefnosdz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aktvubht.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2iykjmhlf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvogcqxh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lojlgnkl.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2inpwyxdy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2aidbluin.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mpdhxzkl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bsyywwbp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2onhplkpa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ihjwkahb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lbtizevi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2evsbejcr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xzldwnma.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dorhoflw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mcictjne.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2zxyeaeyb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jktaoyii.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ktdsysdl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hcjwmxhu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zvkjbcbs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hogyjjpz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gbllekmo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2utwucqwh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mtzyldse.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xsfunndv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xzbpwwnb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vuosifjd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rkyinmar.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2szfzgugh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkscfrbq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vceelnxh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2pkpabiiu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2sqszpwrp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2pyggfnkz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qxsgneau.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nkkjuzqm.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jcmlnqjq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nscbspsv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2oiisopxg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yzvbyjwq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oxcnhkpt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lxrtqyaw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vifgklzr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jwczitzj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2javbdisp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogfahnol.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mlmzhckc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gkjcfqot.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zelcyjwp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2aioylkxn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hpmftiof.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2yebksrbc.html


<!-- 参考信息 -->