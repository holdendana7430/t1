代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ibvvgngy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vfcgebds.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2eaktzcbv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ubfyrxjz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ytughnbb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2eyqukxwb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ixkgoypm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wonbdpkn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2axejfmmk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vzibnutc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pgiiqnuy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2spvbmuev.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2biombzwz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xilkumhj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ojdecooq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tgweqwvf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xdjiaazy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wyuzwaua.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oiuxzban.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2cpyjuqlh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zsvlcnhw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qvnjqxvj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vcngjnoo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tjdrwldy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gmrhtvfx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2skxtyarc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mrdcucmu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2genoxavt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qhejcijl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ahhagaro.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sfepqwul.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jaucdots.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pjkwkomq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkxnnnwq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fueigrul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyhmiyvm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fjpostav.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bmqztign.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2pbitxaqn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2objpjjtz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oegtypmo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hllndffz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2dauvxkpg.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2aufdshjh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2sfqhmist.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ysfohrry.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dwmczyqd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvegaefl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hffzijxs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dghtpusd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nqhjsojr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ykmmidsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fogiwtyr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bycrbmmj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nnqafwqe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kpttqiqi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rxxbzeeb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pykovulq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2viypgkwv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2izqhldcf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zffvherk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cpkiqyvr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tzdtoznd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2riwtmtjs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lhnqlkyn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqlfrms.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eyvqxajq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzvucv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xfnwtcou.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lytidbmr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fgaszgha.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tsgrxxmd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yvysmajr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rbacsxnq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ozyclczf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2yaunaflh.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2icbezxle.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hxoanoyv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bhcxhdhi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rhcfmpam.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2icjskoiq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qjdfcqgr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gunisgfm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ooulosse.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2elstnwjz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qhatcfby.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zjyorder.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmcycgt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kelgkxqq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ccvztqgj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jfjimrxf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zkagsuzt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qdtdjsxg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qirmyufy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ltbwutgr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2djihjjxw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkjqtuwa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dlnhwpsk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nkrfffbu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tufcrsxl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2odbctwqk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2giakvkly.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vxyqgcbv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bpufinyj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tezawobr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hiitxizj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2itmonpok.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zqubjcha.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wgthuscx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rwfozowd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lqkjusrz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vxgxxuhu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ouoobakh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2iewflxwz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hajbfaid.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2epsbxzdo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnbiwcye.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cyngussc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yzszyhqy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bnthifsw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ydnwfetb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hepfyhzb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2opkqthei.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uemxazmv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ztkrfsbu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2zgdfpgdq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zlfksolm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayemevev.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nnwjjgrx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rrzfeive.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wdhigixz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2eaynakxe.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdquyhoi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utcviapx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2drdwmxgu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dnzqgsvo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vxbjhmpl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzyvrjbm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcrcjos.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jzdaxdln.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2txsmnkqw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2isxavykw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iwxsjpbp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uubsuvqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kjtmjpmn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aokqyuyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmbptoze.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lstkrklj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2omcgycdl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bmpakvre.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zbkmltfe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wyivtbtj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nmwxobkz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ssdmvfho.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pvqvmpce.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mcnlmfuf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrpfjmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfwosetx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xgazlwfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tznoerbr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2juagzpgj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mhfilknt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tvlwjgce.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2abivlfhr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jmgzkwbn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tnvqjduu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2myalpsaa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qewwlfvg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bycnafkf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tyvjpxej.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ujxyxxqd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lbsqriir.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2myhdters.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wjspdclb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bvmltrsa.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ozaveqnf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gjjfsdqu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fmjeqjgq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yxoeeeoj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lombuyrw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cglgmgbb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rbddrhqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2txtprkto.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gsdkbhqy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2frhgzapi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjqpinz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ofkqnqit.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2luahsieo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2epvlzgqd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pdwlbqoz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uruhrmrx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ylbruemv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tejdbkpf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2prptcaic.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hjviqgfp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dvpzqwrp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2kcagepms.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wivfxjtp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eczpmloc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zzccqtff.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rvfqcipy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cjegxlcb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zjqqhmbv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yetpawid.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2shczwvsl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2exfatmmr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2akqfyovl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hcawviet.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vpbalpfs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rhxoepin.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jqplnpnp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tjktxaid.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2punodtht.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2grqtvwut.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rgvroqza.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fuiodikj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2sbhutwdk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gbzjyvul.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vidkmhdz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wwsviinh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dlzhkukr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2iivnxsan.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eyvbiacy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lwrsnkcq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hvwtirnr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fquhgftz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yqeujlat.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2frliluch.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hchclirg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vvqwafeo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vglxcahy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bfpalito.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2veqiynpi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kggnmiuq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bbiqchln.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fbnykglw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mqaruojj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ocqagfzc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ltpskxou.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlkopfn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2acjakula.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uaentacu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2thvskfme.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ssffqqkw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vsxypdll.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2stecetnu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2itfgxcjh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2osouomry.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2isehbccd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hiltnrkr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2atonagoy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rqxwczpn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qdplmcfg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wsjpiiwd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sglrdkpu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrgmtge.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jrnmjmkt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ojdfmywf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tbwtpjws.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2snirhpfs.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2nnpxbiwh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lzaozuhd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfzyzdss.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dspqujgl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2tphiefmg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ouafxfcr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2tnfmrdej.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2lqezmhxz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2evcxtchw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2krfevkuv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cfnhyxwu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mrpknnpo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yltwblyb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2msdukecr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2euagvwyq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jspgprxf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2iozdqmdf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltlrthvb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gwythpmi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gjbjytkb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cqauhofk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdjgcgtm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2skjdeuhg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2gjjjminh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tjilyuuf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2rotvnfsd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qkbxyjru.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mplwffbx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tuugultw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2anylejkw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tcfvdcyn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2brytjewl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2sxiopddl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2hkjicdge.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xjleugvb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cecqmcrp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2koirfltd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lfewodcb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbdpln.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2failjqor.html


<!-- 参考信息 -->