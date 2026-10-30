代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gbxemckee.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gobrauboj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gwpqguxov.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gzojvmozj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guctvgkuo.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gvrczwaew.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gyqhlslvt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gbjattzse.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gkdhhipjd.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/guvqsurcy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gcnjcoqcm.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gtenvzhcg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/ghikmrncm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gpgzgwrer.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/goeagzkne.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/ghmnrsyko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/ghkhtrbvq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/glrnlrgcr.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gmuecesxp.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gubltbpgs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gbwetyjjo.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/geqilvito.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gsqhzfoic.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gkcpaofdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/goztiondw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpxkchroq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gwhdpeasr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcjykkjsd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gonrbindp.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gfckbtzci.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/guhqbtcgx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gmqcdwceb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gztktewjk.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ghjpvmkrt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/geewacrrc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gstnlgpai.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gllkxcfdz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/glewvlxhy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gvdwzidrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gjpmuzbvc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gpobcmxhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gpapzjeae.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqodosvir.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gwealeyjq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gqbhjbywm.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/grdlcupla.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/glqehoiur.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gtqqipbau.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gorkacjhk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gtmjcivol.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/geqhkfavh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gnujxvcdg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/ggzldbwit.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gxoykpyrt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfbcvyj.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gdrtecbtp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gxrzbdzin.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gohsezwpt.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gocpnbwum.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grozzpfhy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gbtenktis.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gjyztkmzr.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gkcdfntdr.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gxmdosddx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gchdvigkn.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gkgysnond.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gpcxrznaq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gfrzyuhoy.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gguxuzbpb.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gbhiefrmr.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gsbssydep.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/grsbrnkfi.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gvxdywcjw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjegkxhs.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ghjyrznlu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gxowflvvo.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gqlpsprgy.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gjgoempqi.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gyhidbmva.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gimldkyxs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gkhrjqhpl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/guiqhnqxo.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gyicprzwo.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gwudboqug.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmeefvlvp.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gbtkxutjc.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gujvdkpnq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gcpqtyyxw.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghqlyorzn.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gojcdnjpr.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gnhfbtpyx.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/ggovqqxyv.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gmfqmtssv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gvcqifybs.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gezahsowq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gnjuxvvoz.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gqowcengu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gjejblfye.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gvfudknvn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gwemdijhm.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gzdrmrjck.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ghuvluuuk.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gpugiqwrz.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gtkdpzdem.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/glrnwriho.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gdtbbrwbp.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gfinimepk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gokwbwtgf.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpdrkpnyn.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gpfqgyrwq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gllnebsxs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/ggdvduorz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwdpwdczq.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmuaipgoe.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gfxxhmldz.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gsxrswuco.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/galuxayue.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/guppivewr.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gsjipaqay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gtakqjmoj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gynyuxlwu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtunycgfh.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gsmroryds.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/grbdsnmtd.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbgprhcug.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gpznvgmpf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gkwomcxlw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/ghjghmgzs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/glvmiyphx.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzqqbvflw.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gxjklxpsa.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gsudasaxv.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gbbsffxfd.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gftjslapz.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gdlyajikw.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gitihlcjb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gjymfytyo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gigihdmle.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gppzvminr.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gzzldmsyx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gkvqkygix.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gcqfqfils.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gjiosgtzj.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gggoratoy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gqbteouvk.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtaqbppyo.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/guihfuyee.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gaypwtcop.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gdmnsxdri.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gajekggrh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/guwxikags.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqsigbipj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gxnyacpcl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gnfnllime.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gwcchtcfi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gdrwvbmcg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/greqggkxj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gjyramiyl.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gaufiynde.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/geqiexoyh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gxjbpzjry.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnbkneotb.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gcqjpcnxv.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gjqumtdjz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gsqmwsfmv.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/ghdllxzek.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gtscvmxmu.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gxgnzxlnm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/ghimkywtq.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gwoblcqiy.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gvpvstqdl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/glprpodns.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gjdpmjhxl.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/ggedbmgtw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gtrjfyzyn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/goetskpvd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gvzhsczbz.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gfkykznir.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gulwbimbl.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gifmlprdc.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gsdkdgqal.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gnggmgtbg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gzmdgvvgx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/govydbfik.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gsfdcdmbk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gfavircsp.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gxnthdodq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gcfjchntg.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gjftuqxye.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/goubzwxac.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gieafvxon.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gdmllxtud.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gbmidkdkq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfszbtn.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gwzijinsw.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gyzxlhpri.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gditowpsr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/geseuxuwc.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/godhvtrbh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gspmmtmsm.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gzshhiklm.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/ghdtgomcm.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gapruitgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gshxcayxk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gylynjvfg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/ghzlrnamt.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gpnbbemdd.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gyfigdvsl.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/ggerzlyua.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gpltvnquc.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/guelqbsrl.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gihbadbwi.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gtkmrvfzu.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gzrtxyzru.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gpcfatcdb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gfrqhsmsv.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gileygqrt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gkwofjewl.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/ghquvbpog.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gzpdfqnvm.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gynrbcwrh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gqoraalao.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gvldlzhom.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/grpowjtua.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/ggjyhyeib.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gruzvqpyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/ghykiwyxn.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gvvwhndcp.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gskuauyjz.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gbxpwghsl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/grqacegmp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gtamxtcbm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gmyjcobse.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gsydxjwws.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/ggagjvohj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gnffjtjes.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gzkhmnzjc.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gvjsqofdy.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/grddfcnjs.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/glqtgickn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/guxnvhubz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdfmnfhju.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/ghhvweqdh.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gxawktghp.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gjhxiommy.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gelbrnrmn.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/ggpzqpvpi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gdtceclgb.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/ggrmugosa.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gkhlpdchd.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/ggkivrpib.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gewgswwcm.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gfkyfhlnl.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gfrnooyng.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gnwhekjta.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gscrvjlut.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gxlsfnkoa.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/graneubnz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gfmqhmjvf.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/goqzznvkd.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gxjlkvdhl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gewyjeulc.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gjkeivcrt.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gyziaxebo.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gyexzjccx.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/ggbqyldtn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/ghxmqnzxt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gjkkpnome.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gsslovanq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gfeckrixr.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gxhzcfdnq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqzpmbj.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gzlrorqzg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/ghvqktywe.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/glzitggjh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gvzbfkiua.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gftcajysu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gaecrzowl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gjioktvpt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gnsjqlqaz.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gbtblscgm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ganfvrmzo.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/givvpqywe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gytxwvkxi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gsfoqbmqh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gnuduqcqm.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gpmgvyyxa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gspzmpfnr.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gvvovnyjk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/grtjxushw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gpyxcesic.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtlbbly.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gqtlmkjot.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gpgodjjws.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gthylmaxu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gleteexat.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gkttgzctj.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gaoduqmsj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gyoylrmhw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gbfncemoe.sHtML


<!-- 参考信息 -->