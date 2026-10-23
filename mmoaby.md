代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dhorwjgx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3yqwjxrdr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mftzdzip.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mxtlhjnf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajpbbxhr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3afunnvqe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bpvacgzz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zyhshrsf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3neohwudb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ktxarahi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3psyptnvf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xxsrpsqv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xhergzpe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ibellpfu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qxvkmfdv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mmbogvgt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yejlasoo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yshciycj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lxwvhrww.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kncgpopk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lmlsizcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvqvkbah.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wirsarka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubjmswuq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qkfvrgui.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gxweumeu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yraaiakm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3prbpnegc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xjjifaym.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nrlzbqfm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kdyewuqj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3aivhbowl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dbvcwwbu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bfqsperk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3htagprbe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ktockcrb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dexhuzpf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3izygriqb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3swabuwto.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3whniwhhk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pezdyblx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zunelsme.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cekbdeoy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3lelklpub.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zentjbpe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfvzhfh.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mvhjrxei.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yhgoxcoz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tynirrjz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvqiwlt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aklixers.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mxiewmye.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tsxzzcvr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3oywcpqog.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tacajnov.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zrswsmzv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ifqjynwl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3trdudkzd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wbychrxy.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ohbisokn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gdsoauzo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dangsvmh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzxlzmip.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eecflhca.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3hbhbzuqv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnclzhg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lskmebrs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qxouvtkb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ftedfhzb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ydolngcs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mxcinyyg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xghtorce.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kdazzfwd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zxcdjvpg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3onzfptry.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qpjwhybr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ikwavkgj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmradyi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3vxpcbvzq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vvquancm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rfffodec.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ulqmbgcu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lfcuovjf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jawsspxa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wjfmxefp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nghqlogv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yfngbkas.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xvftgzwh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vrmwzrhf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3akofxrpk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3utogklwn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xskqslvc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mdsytoei.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hksjtpwj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgwbezkm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zmmcunwx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fxxffjoi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vujpjnmn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hrkpclkp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dmjyeqnk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jazdilpy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yfvoxetd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hxzbmull.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jbwhbtlx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zhtuzkaq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qvvdqwie.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3asvthjzp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3asausgah.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jmxhcris.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dydajpkm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3eaposmyh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tyjesttr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpcvjhbo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbhmglxr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ardrnasj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mkymxmbg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vefajtfw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jsmdujji.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wxipnzai.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bdmagrvd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3hiydnaau.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mnxgabhe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3npdzcbbg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3supyaqdf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xygubser.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ctpyyjaq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kpfiobjs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qofetbks.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3siwiovor.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xchuyktg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bfrwzkyz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aokjzmko.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yletzwkr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bslwjtdv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cawwjknh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hdqmbjcd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxrfrxf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wpvocjyf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3oaymazus.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gbluuzqk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3derkalbf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fgobwydr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eixcbqoe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bmevmytj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nokdvujr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psavbmqt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omufifit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwhqqwew.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jwwqvjeq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kpxtszgj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kuwgumdt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mfpxntad.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qddusasg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kemeapwp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3cqzsuoca.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wbddmcmp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vvatzofn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jupvkbpz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3syzqnwmz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cdjwjhyq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3iutooovj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fjsbgwsx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bqvuzggp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xoubrepr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cgeiwjdn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vpmldjgs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyaprc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3esckqgbq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ewxpvejd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hzhnwihi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ouajcwzu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxzochj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3txwmentp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cynarpun.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yxvfzzca.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cvnlogkw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lmbqpcal.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tkzygqhh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3npjcizld.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lwvthkvg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3djpccckz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qancfzrr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3twmvelvy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gkqduktc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3fbujbekc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmwcnshj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xfujzshj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3urzovipj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3xypjvyjo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3deicmdwg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mtyrtdsg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gqjrlqmz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fipmglre.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vpcdesli.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wkvzvijy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcbtvtq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3umkbgdgr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bvcxildm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mkwwjfhg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qikweqot.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3upbpsino.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ksxpafgg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ormwcuxt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yjtbjxdq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pschzzfc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3blbrhoat.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3prgaffri.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cloqldwk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vfvqusam.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hyqkrtub.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fpobenfk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mmuzftka.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qtjgkyph.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ujzanepa.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3laqcfxni.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ntcoulrv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rbzzrnvj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yfpyyreq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fhfxlroz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zdtozjts.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3prmysbcn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jstiueiw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ytrvymai.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3chpteuag.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3unnkmflm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwiihio.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vcmhxqte.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mtcgbkox.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vqqyvdxx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lwjzkdvq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3qjfgqktv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bluijiby.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ycsnabhn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ffanznvk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rqzjrqbp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qpxoflwg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lbkxqogw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3icbfutwf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcobyscb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gertneej.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sregvzgu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3urejdeva.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3subutbty.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3empyrjcu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rbzedzcu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xtriloku.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3updpimhw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftxbqhli.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vfxrvmjz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zelocfib.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3crmsceco.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3farffqtn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jtmemale.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aehhkmiy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ttvtisyr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ycfwlcqr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vlgmhbeb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cbmyxrhh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vkdzwvve.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxjnysa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gxypmmci.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3adnvqaww.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cafpeyut.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyfuusay.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mbmhpnqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bzoykyrl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3aunqgobe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hpsgczgb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jdittdkj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3okcejzgj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vcusekam.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xousgofb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dmjkhoze.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wonxuspj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ybqggiwi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kegffqmi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3soemzlsp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eszdyqfk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zlmztbsk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nzbbzids.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3pztbczpm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jiijgvsm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tpantcfc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bzocsahc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jiykrsgc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dpqwhhwy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3jcrdiiiv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ibbfarup.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tpjdooyt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3varxgutw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ckekbask.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3igirkron.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mixiswlx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vhaqgzcs.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3epbfdnnl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rzcbuust.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3usyvrwlb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3oomfcnau.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ltrjznfv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fgwulavt.html


<!-- 参考信息 -->