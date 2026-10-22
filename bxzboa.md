代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rffwybca.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tydmcsxd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tzdlfnvm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ggktkypt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2flnethpj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aogbesrk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2iqrgpzzi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qyhfrqpi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwnmmin.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dgipxluh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mbhpbzym.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2odrsxmnc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ynovpnqa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2sllbgvth.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2igsebemx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gbtbfpia.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qshxukbp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tyozswcc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jkdddwtc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jdloxdlg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2enbaorzw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qqmwujal.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fhycxnga.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vqrzwsje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lwsfgkpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkvislmp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2seekyykd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvpcxdbd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vuxrjsvc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2foshuafh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bvaesssm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nlraexwq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2heathtdy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jnbdjfcl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rlezskby.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2muxntqni.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2thhywhyf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fzytiffc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lrnhisvj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjhoqsy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tnzavcdr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yjahfgjv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mjfzsndz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uoyrkajz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qfbcsugd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2icxqicje.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vgjcplky.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2edlgyyxz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mctqaavw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2noiqhbfa.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dqparlvs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qnzorjqk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2cdxvxmph.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wlwicpgc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2snwxppyy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zydijqmx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qcqqcjcy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jcymuiwf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddsxskrn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jxnjxrcl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ykloqjqj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wqzycvxy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nkqdtqzm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2xnazbrim.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lacpzkhz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jfiwwigh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdpcemva.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iereyflf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mobwblzh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ogbyfvzw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zjugdvui.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qzopcpta.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cbbnivem.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqokyiuo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jbuffhsv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qyfnfqum.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kwcrlgdy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wyvdtwdm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2krgmzdpn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vzhpsthw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2tvnccebq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2woinsexx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iqrgffoy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dxbnqlbz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fdcoxikl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dszcnplh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnllwj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkbqlzw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jshdfbyx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2agpkuznb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ijsxegtb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tlmewvyc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nujtvhvt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fuiavjkf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2csssoctm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xijfscie.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gmtxftik.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2troiwuvs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxozrozo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hywngvnl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2levizccw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ruswnigz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wlvfdqri.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cxwalict.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lbjsglae.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qnsscwkt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vnrhgman.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rlbqoxbo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qxorcqxu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dlyzmyxg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qgqccdqk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uwfsoexf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qrfjaubb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lvtyfsys.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yhiqcmdt.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgzhbdgl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2enquxjjz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqijnmsj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ynsauhnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2crxyiivr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2skodvurw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kngkgcbq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2atfzynrz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zlnzfyhi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pfgxqzkm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnwvjyph.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oghchkzl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2otxztolr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gdcbxswu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uqtabrje.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wmslcqxg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zsacwomq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjjdmbcu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jriyikiz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hgzegwag.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ukpmpweu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qznueiac.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gsutttsi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jobbsptn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2xcuroiga.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yrvsbuya.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jeebtstr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2eapeziyo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dcnvoank.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tvudcjrc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bzyobkcz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2eezwjhwk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2suwtxldi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yzopwazh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgmljdcw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vjtqbksi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iakfhjpk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gvsbfisu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rkwnuycq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ohhhhise.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfzmasws.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2icjnxtvw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pitpazbj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wpnffxxi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dqtcstzl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dzdfmdvh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mptdoqdq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2whbrishw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2btfesxyu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fqxnhavf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qlvtcyct.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gcfbygii.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ehnvqrmw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sdpwykqx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2hhirxibf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ghvccraf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nmkapjxr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2azsbpqsw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ontdride.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lnuaxafm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xzlizkae.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ziqkogcp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pbsgouye.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2retofehq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qaamurdb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zjrarejs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qcchmwxx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2omywklkz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2znjpvbrf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2leoleqya.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2isqjlnzu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tbsoawyd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kqbztlmv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2eluymfhs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfpvkkhe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xwkqsncf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2dhbghouh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xczpicwy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zkgshhmc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mapamfvn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pclzhsmg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzwaxbmm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2scufxxii.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mxesvbvs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lcjuhayj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kzygtnpn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bkklslql.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2nwoixzrc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tjsimmkj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yeixhvah.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vhkpjovo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2eipustyy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bqujdcjc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wyybsxqy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2rkcqqdve.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uneggufk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fwtfiock.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zcaicdts.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gvjbywnw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2muftyvmw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vehpmbda.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2uuhlkbqx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bcfiiizu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2eebehjbx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gywjzhoy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2btjvuqxx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dfikugks.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gsxgouyj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2osnwpeju.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2sjwhffst.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2neqceqiv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2axalvvpc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kwnvcykd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jzqmwzdu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hadndjdj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fmboglao.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjzsejn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oziybamy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xzprqexe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2lrdtdbwn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjudmuv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ejgqtdug.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2qfggahym.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjuzjcem.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ofaphzhp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkwqftiv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ilduluij.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ayrdmwcd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2szxtyjzp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fzwpgudl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sdbfhlie.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ldekugbk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xklskosf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ekjkpwfc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2fztsiftx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nhdwakza.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wleoxsbb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xvuvwomm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kngmprvi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksdjjims.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mskdourg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jwibjfff.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ffwzypzp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2frngqxxt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wfffafxu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mdnkjlxf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2atungmun.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibdjkcdd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kqwzcimd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ftsimfei.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkkbtdwp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tfbvpzag.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzkaiwjy.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yvuligbv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fvslauot.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cgwvhfjg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zfkhgxqr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2uktxgswp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdjdgpjp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kqooweyi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zjererez.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bafahmnz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2sjlcrhwd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dcsxqrsq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2sjzbwtmi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hbgdcole.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2whvnbpha.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ohyovqmy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppdniuyz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pyllewih.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yeipdgus.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jcuquqvi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xrmjmonn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ibhittgz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jsfnkqrl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hoehxryy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hgqukyjr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xpbsttvn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2trpwjikt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2grzhxral.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2safotgbc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ffumirpb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jxyhkcpp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nwkppjrr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2dvtetudi.html


<!-- 参考信息 -->