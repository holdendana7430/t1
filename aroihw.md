代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zszwjrhi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ggpyynfj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2jsrwlqxy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fliftrnw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxzkcnew.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wfwaaqqa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2peraajdj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2iyqwwrzh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yuuvhxvb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hrkktfkg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dujlifkb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gwvavcob.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xwpovimp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zyuthncl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2klejofrc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2azitanoc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qpmznhjl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ojverbsb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fuzpcoom.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jwdspvbx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wrgkkujb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2utxyngut.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvuyqrwj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qysejxzv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pcmxkstz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2warkjyeu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jqhehsfn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cenecvav.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqneoiqy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gjgybcpz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zzsvxzek.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dgrxdnzc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bebkoqzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqvkiqgo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2oiyddwtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lglzjdhc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zcotxwtp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lilowiht.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnebemne.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vindgckl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vcsmjtcz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bimmrfis.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2muwoqvba.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xycwxfjt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yxtsinyu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dnogxlcr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ujkvpaee.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lwinunzm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2objknlin.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ncaruepp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nhibuotc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2eipoalao.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtunabbb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2vjtnzwvm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pefikubj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fuzbwwef.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mcqawjqe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bneiuhaz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2euyismqb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2viahpaoi.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2absjmjzc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnpikqe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gpimogyg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eyzuvkio.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tdeqfiig.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2btamelrj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xmznevcf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mgqadqgt.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2otxzpmdc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ecvsjkbl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zraldzuw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2elrzqtmv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hzazxzun.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lbvebyjt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tatthjdx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ljuivnxi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vmhdinzu.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rpdgsdvu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zcqalmkt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wwztmvtu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oousvhsh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zromotip.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2felctfvf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvzpcylo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wecgndri.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ngnugkip.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xqjwjxga.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vblctdeo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tntpmbbs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2hremkggb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vmqbejik.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ivqxrdqd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vttodjwl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjpfwd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nfqrszwu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2paomsper.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwspcjlu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2reojjrmc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtkjoowy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbutpbem.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mnsxgtsi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2txpucgjg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2wduvkdwo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2uoxumauz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zphgxvhb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tiaqdagj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikxeeeze.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2rjgbwzxm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ofhbcdow.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cthaabhh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oddicuus.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lktrxiil.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2slhinhgn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nmwydtec.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2taiutjlf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cimhoanf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dvqsdjai.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qgebpont.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tdwpeehh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rhiqobky.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mphszywn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pvnybvoo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ialxvubg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmdkgayy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wkmkcvqd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgnnwats.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bsdhgjqi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjeucfid.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dbowtuzs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pgjhdroc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ftzviytj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dponjwdd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2akmyhdsg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zgqfcoqq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qogqnrjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2scwhfcbh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dpurcqbj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2biuvfiuf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gysjirqk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eqgynzxf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xspaimvh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nxralhgu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ypfklltz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2icrbqmch.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hmzjdiqs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nhiqemin.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhclxab.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2edkqzksh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cnlzrlmr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xmusfqxb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xcvgozuv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yyapiswf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hezdksmd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qpowyhak.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mypotoud.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2holmzztq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cploivhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qikepdmi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wplhajyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxxwlnly.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2emlyonph.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hruhchmx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rvtowckl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jnxiwznb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2doxgkelc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tlckxotr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jhoauqgp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2itbatwzs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2smyedray.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pdgevpvo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2oyfpnadb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dnccrgdb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wlflmxdd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kzukbvuy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2glcxyimp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lasrjhvw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2brfmrcpl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xilbdzyo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dbcwyzgm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uahajnfr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ujuddkdn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpntbgr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xzxiumvr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytcchkjx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zvfsuaqf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xodjzear.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2yabrkhdl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2swkbzinm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2sbnhwzhg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mvlqanju.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2blxnpicp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2clqtalzw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xvjpmbzo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gevgstcr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wombvchl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ewadyojs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ajildevf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmovtti.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hsdahubw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pirowzdp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fwoaaifm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2neeuvgse.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mlerjdul.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fnedlvlj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfzcjqvt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uqwrxwzj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vynocypt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rwuirvxs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2iiemnnew.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jhgsubgq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2edinpsxy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2rgouxhds.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2grozatmi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2khzlbthz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wkkiyboj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mxczkdyw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eqcpsaug.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2miemiygc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2msumxkjz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dueeeptx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dqemcrks.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wfzwnpoc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2oudnghmf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cyknjbyv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2orhjshsl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2isocjfbu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ewjmaded.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2opzkbbfs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hislduxb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ksqkirvz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kwfhbcmr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgtdqmc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yaxzidcc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2oynyylrq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ymwfmjzb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tyrulfhx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2khfovtsz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cboafkez.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jgbpwctc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lsvkaown.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gwydihgi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ubuhhzfh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fetndlln.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vcjsrwez.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gjuwqplg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2flpennda.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hfgbkolc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yzmkrpvg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2elgqzofy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mifxecwk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zlhvsefl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bsppgeml.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjqhkfzb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kvdfzlix.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kzcvfgzo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqqrduje.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2tuhvlxgk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2xqvijary.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2iwwwhsmd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwxfikib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fxsbpxth.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2embhjndb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ioighqvs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2krdfdtnb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2preaqwso.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xqjfprxw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2lckbyjkg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pebfqink.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cwnruuur.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lomohxqw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwldqjuw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oucnnsie.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eoumgaxu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jjofofwh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qwzrhcxi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dojqqpes.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vjqfuxqi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gpepzpnp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dotgubkq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rmaompks.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vjdzynst.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvkqyzkb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ilxbemnn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yfiegiyd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qhzjkxpd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wskgqbxu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tajfeffy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nzwadzsl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pqtepfka.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhpnsysq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wfueobqs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2whutkfav.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2oxozmrqk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dzdflxzp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wysjkjaz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2lomkvxda.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2txvttnvc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ovunkwwv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2waunmjau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ucalbyzd.html


<!-- 参考信息 -->