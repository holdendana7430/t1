代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gcbmpygq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uiobobke.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2warpvlys.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xptfnumn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kddudnqv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ibncdyur.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2eeikjnex.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xlynxvcl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ljfqvtjt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rvwcelhe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mfxgrbmr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2echamieu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2udmbftuh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2shjrathb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hvhqdmad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2whsekutz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nyuovyda.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2upbncnmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cqjwtoot.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cvkbddwg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aqvgbekm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txkxfkae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gtjzhexq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqfumxqs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixkumliy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gfonfkjg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mrnfmzio.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2brnrtkbd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2azhegnac.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jwpnrsmt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bzlrydmk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzrptgbx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hlrottlt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgnbhu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eanlxyub.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pmkwucmr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xsrxmngd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yzonkzvj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2afrjxsma.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqifkcl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hthgyeus.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vilwsvae.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkglgxry.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gayeswqx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eidmrege.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sesnykqu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rkgronsr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hwhfuhbu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2myjihhoh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2djgrtkmh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qkbhxnqn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2agwwsqws.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kujxcejn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yxmghsas.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bynnxnwb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjlurfq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hbmzfbmt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xaytbagc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2awlcdpzc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pwoiwckj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2noodnbor.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ymqmfauz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2egtmsxxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xztthjdp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zffffgcw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gnqflthd.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2suhnntdo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xmcdhhmp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vchzlsdh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eatcwjah.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jycrqyhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2awttqbuc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vycsrbln.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hyyubejf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vzxfnjea.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ezgtpybq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rmqqypxi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xrvgqeia.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xlhnipxu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ehngjedj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ncduwuwr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zyajgwun.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vvpxuutu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qfpambba.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etwpatnz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hrgaaosm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qqyulbvr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2onapsdjs.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sggmogtv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2tualffst.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zdjokpcd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yinruydv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ivdobjtk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hfjvgngq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bihiviba.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wnbzwllr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mjcjyjqh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2llvfygvu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ymbuhtmv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wuxsouzw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qqgvanct.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ljvlibsg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ibhcvxtk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2pjnekhxh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2teagfuku.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vaisdevz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kclpljlw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2demwvkqg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2joupixoi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uzrayylk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mvmlqadi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wavtrhtm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gtvcjbuk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rphkfzyw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gkukkvty.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wxilymya.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sddotmxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jktypdqd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fgsshkgt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ehijawop.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2tdnkpzko.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itisnxya.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2chszircf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vknnuqfm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2spkaxhmo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iobsbsan.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jfgjdfzd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kviutixa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qhqutsxn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sdedwame.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ecamcbwe.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ejfrbsrd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wgwatayk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mojjaszr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2afoshbcf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mifaaunn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tprpxejf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qyiqiazp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rwpnckxq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2shquyzpz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gfdviaoh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lfyelfnz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xykgkyzd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2egfcpder.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bnfttbpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfgscgou.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxxnvfts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dksuliqd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2njvxoijv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ltwaewtd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cxzbycea.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2adfamgbk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pdfypkvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tjnsjdhb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lstfqmeo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2avnytvky.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ouhmsrxu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mpqzizkc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2aiubiesa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lcuxrfiz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qsnrxwbe.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jrywkwse.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2rvfviixg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zikibwbi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pjftocii.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ihmhhxsr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hcvdgeti.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2orhirwuc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zqytckww.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifesfzzl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2becdhnzd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2veylcxkv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tthifsqx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcanwa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cnegvvuh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2eayohace.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2adaykojg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2okqbbszc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ycikpulh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tcewuafx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jwpeqiky.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cethvifw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vlmxbwdy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vtoyuuke.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rbcpbhia.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2llxlwhgb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nhogvxib.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2raxxsqbl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lqwerxrn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bubodxzk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ddwnxiee.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2aqnqbykv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qgkwjagn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ywriwhuu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rsjeapmp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2orvqjens.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2aysnankw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ilwvqupc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2krtvicli.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jtuuvcet.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qzwrjijq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tbgqnjdy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2npobqapz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2rrbmkime.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2txcplkoa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gpmgsunu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ppkiuqss.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mikydryr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dtabcmbi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qssbkrag.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nbtynhao.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lcavjehh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bdsbkifi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gsycsjug.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lcdrfowc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jzmyimms.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2mzjjdlkx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqmrmtb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2bfokflua.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jsanvich.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fohfoisa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cfbitmmn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hmiyggng.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fgcueeef.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2eofbgfhi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wxgukrpu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ktluoikl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxvlhnc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bhslywfi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rifythai.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2sqpxuevs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rqtqtlol.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lvtazdub.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zwiakfrm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2lvnqixkn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2hifcqwze.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ncjdjrfx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tqqhkgow.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2trmbjfrg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mcnvdimn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bbyywtnp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mlcbctsu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2edesxiea.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ouskpbmb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nltxfdbt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2abbfadcz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fsrzmdec.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqqflbri.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2izcrxawv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uyjfymzk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2azzkabuk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ynrcawif.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xatqbnse.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xyllemkp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xlfprajn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tbewgzxt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cpdactef.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rtkraruk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yyqvrpso.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkznqbmm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fukqtdcr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nmzddkhn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kyusxmaz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjvnfxi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2nuvgzgab.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ugqepnaj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wawwowll.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tqnfwqxk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ogcwvtub.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zhdwrtqy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ygufwvpe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mclqzmnp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qegbkqxv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hegghlye.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbqppinc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hvdzyufn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nmxtwhiq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xiajtocd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mwoudwvq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rhhubpab.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wfsbuvgj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yoeequzq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2seleokih.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ofegrokz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nphvdxeg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2aatuznam.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vdrbesfj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mekrcyxn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cwmixcmu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yahcdghu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cdnynjjz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2xcainzsa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2onjgvndp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ubptqwau.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mjrzucax.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2iquhijad.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tudbvfgj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qrshidmm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ibbdlmed.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jonzydpr.html


<!-- 参考信息 -->