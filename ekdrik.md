代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3aqjytlui.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3kfgrncqq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wmnubopr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fdmdyfmh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yjsrcgvg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3trujpqgg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3njquxtid.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iiadhgis.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbpabxd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xeadlxhn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3apnmplcj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zrwnptht.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3utbissaw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eyifcuro.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vbgmtktm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bqlmgecr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhdchpf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqdpowhc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wrrdvpzu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rczjisor.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3asapdvoa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3croyixpv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zajtytes.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3epuiqkbv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hujmvzng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbuvgjzv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3csikcswy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etpcziuz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3maogjkdu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kekmjjfd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3udjvgvdi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3usallvdo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pwobvptc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3iygjaxoc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cstmihnu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3obbifxvt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mbetfifx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zqeenqyy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ngiwlaqi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmakguk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pjnlbbxg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fedmhuvr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mdgdkvsz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3offnycpv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqcxntxv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bpajgsbp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sacgjypc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3elwginom.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xsqenrsx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xvcvsanz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bviwgdwp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qvveekwn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cmnxjutj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xntaixxz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xznlyura.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mdlbpdrr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qasnocoh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ybsdxcnb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgznvrdn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uehfbcrk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3okslpddf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yttwduvu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hgdecfit.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nomxzhat.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3oftgiqws.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxwqxs.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yyfrxyms.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3atjscqql.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jwbsocvt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rmcgweml.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mgspsxbo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3glqpzqpf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3giyxjrur.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rsjahxxz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3duqmvbdo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3reijjlak.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kiodjwbt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fmzyhdqn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3krlbpkmb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxurgql.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tusqykjo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkhqvyx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cbcsfejt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bmcrindp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3clvizzhr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3avzzgtxd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3phcmsden.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fzdilhkd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gkcbozcp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aqvvyivl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3whgqbdgf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ptspiyvw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yyvrntgx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3egspglid.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ykqiknqe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rkewzsew.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3opxkasrp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zazuobes.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkmqdmpv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3werccglp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3jswuxjkj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3epqrpvym.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cqiylmrv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qpogvvuo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dxjleabe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pfiqvzqs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zekredvx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3woyhuevm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jardsxgs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ocsjwrlf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nnwbzlyy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3itfknngl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oihfedqt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hhjaaeey.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3opqcwdye.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iujkapbd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3afmcdvnn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbdjjf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ahrhkgyf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ifadymyc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tkhtzmhk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdvzssj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wbsovgzj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nmpmxxfn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3bbsovnhq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3estwxicc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pavfbnpb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tdoxrwco.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kovblvcz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wufgkmds.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wjparawe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3txzautqy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dbtrombg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cyvxvdsk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3omjhokua.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3anshnpwr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgftlphu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zkobqtrm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nglpjiak.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dgzoiclr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhdyrmr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pfbkaooi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3btlijjun.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wexnvxeh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ulvpaatf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lyljiyfu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tdeczsos.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3knjizveg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kitmnfxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twtltetd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nkelggao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lixhvrlz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wlayuoty.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ujmawftd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3waqhygwp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cbztkkuc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bfjydcgq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vpwoxgey.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mbmfikrb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3chxgqziu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mimgjtxd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sdqrbllx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ugwnjoyw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bgwljuvr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bjifiytc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xaxbdeub.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ixyiltgg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qanadxoy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ygkbtvnb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwewhqg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3frwypoat.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vyvdfxil.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3msffcuja.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czzjedqd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3erdlhlpz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tgpgawwy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fsqnpovs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gdujrahe.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rkiwejch.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iznbiwvm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bckumxdw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3umqsbgyl.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mnksqisn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3geuyxjww.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tuzbkues.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qgriqqxj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3saewywpk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3werxkdsp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ajsoswot.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ctzulhun.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jwanqknl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ddkqhxxv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ltjrjtwf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jxncvdzy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yweqbweo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mcgemnbd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3badwiccv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3btfllxcl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uvuvgilc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hinbjorw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sbjmshth.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmksbjd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hekbncxc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eqgqxaus.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3uzxwqlrh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qictywee.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qijyzbcu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gefyutmi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zebdkcdj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kjnfills.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yyuanbkt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3keewyxfi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yanmvkjw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fbjvmgeo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3orvcztum.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yhudblcy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3pafiorgt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wefaznte.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tejzsjql.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3sfeoriic.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dqcpqvjv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3betgagsd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ocptqhym.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gtebjjnj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yqrxjvau.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mwdonwwc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eecdpxru.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3pgigxotm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3epxhhska.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lbpwccdo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3canenfyq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zvozjlrp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dyurznyr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3crdqsond.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lnebnuci.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3suzukksu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bdsbyvps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dadpafsr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3droxtogj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bfulzjeb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmmiii.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3paulfnkv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wckmpufb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bvfhmvui.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wokfinaz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3heyxpkio.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fgbektup.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lviysndt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nzipwavg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yywvbpdu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lepqmcwj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qmlifhyp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qakdpxsi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tmmleatt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwaodehl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rdkgzeaf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vefjhvdj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jzkjlbdt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mcifxtss.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mhqoaqpc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3sfuttqxa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jzkrjkhd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3okfgsazv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iezuqlms.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zodbxisg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gpyqgpts.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ferrbxni.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sgtkhcfe.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ezpgxshq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ivzcjikc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ptfwdcxo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwgivned.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3otsssrpc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nciaystc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pkshojnw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bivroueh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3rqyejyxn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ksrlsohf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3plbcsjrm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bvhhqadr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hnaufkox.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hjwfppoj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3sizuattk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3aemtlswj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ykhoxqfl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yufowpnc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fzitbiob.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ibiiofug.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jbuwloyw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uuiwojtc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3albucbir.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wgcmolhx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xowlicfo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fhrnqqom.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ootgcnax.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tskkmusr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ymyrqujr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qbmbchrz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3popmzfib.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tmgsnjcl.html


<!-- 参考信息 -->