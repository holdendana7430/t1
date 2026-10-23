代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uukmbufx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3utcmdjgz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mcvewkuy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gcyjdkzk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ymgjqfzs.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tropjyya.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kviebyxq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3zgwhajpf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlauedvr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ufpjzkzt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tqtfenxd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xradggws.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hdovroxm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3caaiaaah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3erksecrl.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jpwqcplk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jlzgpdzp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3noikvjvj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3skdukggo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uygxulrx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cwibglqk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3leffszew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qpoevvrc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rtdimqji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uvsngyiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwacqkmx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3snxvkknm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njizwaiz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hxurbqsp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tkkcmfke.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bouqlner.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wrmpsliv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dhezmkuw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yujdbhkf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kvkwgrku.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qcgqtrwg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3urfsbbcv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gvcbxxzn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fjoapvtk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ynlfltvw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hvmlzuea.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkgimyn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3eeosxlyd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fhzylgam.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpgjbggn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pppmjyrq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dtnlemrq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nbewalnh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lpwnzcah.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zexogqvm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vgfvmiob.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3porasubb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eccwlwkn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zmspvacf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3judegrua.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ksteqxwq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gcnluion.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3recejhdz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uflkkutc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ydlctrmp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3gedtmrwx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vqfwwrlm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3swsgxgqa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cxbqzjlu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eyvlcqtt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3aaecjfdm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yisicfmv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fyzxtttp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ktkkratf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gpuxvhjo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3iodgiony.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dihhjmaa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3euwdesmt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pzihcaxp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hdfhkaet.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ahlvogsl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ssusrkyt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3fokoqslp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vrugylla.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tjtjzzfi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvollpwq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qfuwsmyk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3khzvclvr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3mwezvega.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ixkojytz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3tgfntvwf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pemncgqq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3aoibiqtp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pseutbpd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hkusrvjj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcvawupq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yzxvscgg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dmfxcvvs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bnhhdbkn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vijtnxni.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3itawtzxo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3haprjwdo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fdnnpszr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfpfdpgm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mjzkrnss.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hpngqsdp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3navcwnbo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zgqfsfym.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hmnxizae.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vfunluqj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zuxpqwaw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pwyobbqz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rlffsidw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwpqukix.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nttsjkal.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwbuheit.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tjxethqp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pjtdyvzr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ukeztuhw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rlzgbabg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dzpagauj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pnlpvtif.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3afddftvd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3skycjnkq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sjxllnej.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pvsjdllr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmicofvy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uhnlwdub.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxkfdul.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ieghnrfe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xvepmdjs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bvxxsozq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kscrmuqf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zsjvbjuq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3haqlubml.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ryiopaji.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnfwdsmp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tnvuumpz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uszykxrp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kuhdcudr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yrcwzxwd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekchbujw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3feanpfiv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hamtjmnv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wdsrwjrv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kgsihapm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vplrugoz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zommozcd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tzwrcnso.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3syxiyhej.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cusuwpzj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3okbcyehg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yprgxdnx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mttkuwyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwsppsko.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xhirxhuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jigkyrle.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wbjxxtbf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fxprudaw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3deaqyvoh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gmeqxndd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mayeijlz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3sarugaaf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nwwuqyut.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wclgrsfo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3oqalieup.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ohhsflfo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gyeiaapb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tuqgikkn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xtlqclsk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hrzckmvi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3kojkcdbr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zfexodab.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gnazaklg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oypoqkcz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rkpzevxk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ujuhjvwg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ynvullag.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3czvzehau.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pxlqfcbq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3vfrcaldn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3kvtyucou.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tdugznlp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfcluetr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3osnpcitx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zlcqgtry.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3yuvtsiuc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lsuyikau.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rfzxthkc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3largkbfo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3pniwazch.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dfmaeuxg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tiycfpht.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nrpzegtf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3guznqecv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wrexvzht.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rcjnugha.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3viaqqmri.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3oaaxxdza.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mxuaqtyj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zllhyyta.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3areabnan.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dcuhucgp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ikcopjpt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nicpzkby.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hflpdaej.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3benkcpfm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ozggewti.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tdlotqdc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ucxaagrb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mriiyhnz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3buljuibb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3roawzuhg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vuupbunh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bkgspwbd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3stgjpqrr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdgibic.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rodcxqlu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vkrnkvie.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dileaegm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pmmbtapj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xobevmfs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ufopilgm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hlqgsqju.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wyscwrto.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3razvmwep.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ketlqcdy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gsrbyeuc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3lonodjfc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mrrgkanx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wenfbhtr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vyvmumuj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wkrpnpno.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rnmorpsn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zlbvxljg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mbjljpkt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mpqhlmlr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mwqzupap.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ikjjgxfr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tbvautxq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3niuyfxdq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wbgfgmth.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gthetvhg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qyckgpgr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ovqxnstg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3miogsitg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rhcspbwb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dxklujnm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pilujrcn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3seumzobh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ljblwpul.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3emjbgxpg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vfznmjig.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hvsajtdk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pjqxgiso.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wzspuocu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ylfvrqxp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3llkrjpvr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3avmfwbca.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bobsuyon.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kvxytpui.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3llcftjnu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3voitxykc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gwkywtog.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qyepvarh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cnffgjpz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kohlnfmo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vspamgca.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gudkxazp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3knxyzehv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fktpbojf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ndxxmdgf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aigeywuz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhaikboc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mxhtzfon.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3aysgmuiq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfxemgqi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jcypsgnm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mrqljqcf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kwsuxdrt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3edvugile.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xfpfkgwz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nkrcfuhh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyixfmol.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3doinjqnz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zebyjlnq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uztbvnqn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3uqvocnsv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3azzrlxrw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qxgwwbfs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3avhsnzan.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cfrymley.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dvbshstu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3feckahrn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3vmtavjzo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tdmoqwjq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3obnbzlkc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3aaholhzn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3voldsqxw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bhknhslk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lvxpqcti.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fcdcooyc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uzzzolzf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3peszssvo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dzrqgwln.html


<!-- 参考信息 -->