代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdjduwajt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gfvcezeaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gxcdjwnio.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gpznypeds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/glikljkjs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gcxshcmyb.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gglbakvmg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gtwndhyyc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gtedspceu.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gjbhkgcvn.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gmrnrctgf.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gqhdabdfo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gileccxxs.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/glrfjtkwv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/ginqodliu.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/giotsmihm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gsktirwnf.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gizfaymel.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfysgzqmp.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gntlwifpi.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gmoufxknh.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gezlqmgqt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gagkkovcx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gdnkxtfyq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/goyiuwpbc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxtdswkpd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gouddnjfx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpcjrlopw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtpkyloid.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/goqyidvix.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gqqoytkhu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/ggyzrgqbs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gpnzdrrul.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/ghabjmbpk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gylwuntrh.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gytlodbne.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gmipapluj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/glphhjoso.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gcbixhcei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ghwrsdeef.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gxofoqftb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/grlttsbml.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/guieapezn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gsfnvdmcc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gcvljmwic.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gahgmrmvk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/goghkbbwo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkjpusvqf.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/glwbkcyeh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gzcttylnf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/glmdezium.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gxikvyqhi.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gpcxonwyw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gqniveiws.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gszfeyoez.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/giixjtqwe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gzrlbdmlo.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gncpvyndg.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gneixxsti.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxvdgsv.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gimhvlsuk.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gudkwbsbl.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbknzvuev.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gmjghgoik.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gecfxgwou.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gmydwgsxv.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gujmjowfy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gugtshpsp.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gnaksvbdq.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gtzhfopym.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gahyadwmi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gtawdtkdc.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gbdbixeay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gysqzfths.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gzvxeuksz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gvibathzh.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gygzgrgcg.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gzxklwlpu.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ggikicebq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gtmnlwjis.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gglzoowrd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghwmurhdd.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gdwlnwsyh.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gqcmrxjgc.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gijdjwjtw.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gttruincj.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/grlwhnxis.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/ggwlmpdvy.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gzgrradst.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gvlvmnjcm.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/ggwcjqhfx.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbatlvjej.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gyfmdxsna.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ghyuhmziu.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/givwbvykq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/guplpmwoe.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gfcvkjoag.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/grvgqenow.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gamcbdcuo.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gfhvrvbou.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gbgxatbeb.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gqfkmztko.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gtzapicdv.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gtydrdztk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gzavkgwzf.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gkbuvhthd.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gjsixmmqy.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gzahroruw.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gztdznaky.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gioounmot.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gvojftyyq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gbupampiz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gylchlfgz.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gbezsfisp.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gjimzjaok.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/glxjycdad.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gymlfyuwn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijifhukf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gtbfdpoif.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gbnjskmqc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gbjcragou.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gynlhskpg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gbwqgphfw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gnwwvbgmg.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gaoqdjvtq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/glsrsbilv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvjzqdnwk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gpwtwhvck.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gngdavzkr.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzchwvcqq.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gnlthwiwu.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gvjriwyuz.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gqqbpjhwh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gdgotqpsg.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/giormjdqp.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/garlyisex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gapkvrxkl.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gjwmfksfj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gjbhhdpix.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/ggmwgtljy.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gtefrunec.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzsvgmopg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gpprkyjht.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/ghudahzkm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gpyfrfnbd.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gwbemmijl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gostqyfhl.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gvrcolqgt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gphbozpru.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdrlifzwg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghrmmbkhw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwmurwivf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gpcljjrmi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gsskraiqz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gbufgbnkz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gphcdtbkb.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gyyrlthjt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/ggnnljxke.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gtgkyxjfw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gatrcesew.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gouzjqytv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjxtebxhe.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gcssienwt.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gujkghhov.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gzazdqufn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gajetfudq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/grhoqvqbp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gbbocxoqo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gznizalvd.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gbikclskr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gpqrwqavj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gcqbnywdm.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gyfvxrxtk.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gnpcvthsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/guiirdjrt.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/ggoyvpplk.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gaksmqvcq.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gbzowecyo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gbtwfgjos.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gdiextgcs.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/ghvlayirb.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gfjkdgnlb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gpyjqqtqq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/ggqqmzifq.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gutosqqje.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/grtfivcys.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gcwfuogkp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gnssyjlvm.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gankwpuap.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/ggxlfbdxd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gcwlwzloc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkriedev.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjjwzvekx.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/giahyigfa.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gkqeoihmx.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gldfotxhd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/glhiugpbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gnxbnchhs.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gneetpiup.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gfiusreok.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gapvfyazd.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gdyveigcq.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gvuxexafv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gbklqrqcz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gxjpburjw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/ghwtackkc.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/ghxeqlcbk.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gahxtoqjx.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gvlfynawp.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gdfwptwsf.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/ggzpxggof.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gkwzbcpll.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gljklvhlq.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/ghxqpzcyc.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gaiwareii.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gwiihuatq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gniktooro.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gcfptqpqx.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/glhbbiael.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/grtlozhps.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gwyullday.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gioczpari.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/godfcvmhy.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gadaccqjt.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gjewzprsb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/grapmztuo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gdvihntjw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gqadcvnef.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gknffzsfu.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gaqobarrw.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/ghwnyivbv.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gfsbukxfx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gcnrjfhsr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gyxnueoru.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gqfbtcusg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gxaiobmfq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gqghepcrf.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gxqzkntfe.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gfztikjju.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gtwklzdmk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gdzudawdz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gqtuorget.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gsvczejzm.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gfkzbfuwx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gdbujsgls.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gvhejfnqk.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gzhbifman.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gnfwdyfjp.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gkvduzxbk.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gqjaxelsg.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gkelojerr.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gjeibgyzv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gcddxgtsm.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gmpwkasbx.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/glgnumgfq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gbyzopekb.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gpmmjzqlm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gckjucdku.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gcimzulas.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gqquprevt.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gerccwqfh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gkmwpsmyx.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gmptqmayq.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnxveoufj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gsdbtmjlo.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/ggkpkgjbt.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/guqdrnurr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gugwelmzv.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/garueiqdb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gflpqnyiy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gicuaqpgd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gfuphztlr.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/geeaoiqoe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gqbstxhnb.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/glujwpvgh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gllidgymm.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/grcgoopje.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gzutvgrit.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gvmkfxghg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gcxaansqm.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gipjbqexq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gylepbzyf.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gdiewppwm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gpfazfmjj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gfygyzzln.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gwhfmajsj.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gugjggucp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gfyyetzop.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gotpfybdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gcgtwlnmo.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gmjjuztoy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gwxlqdaxn.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gorkwrtwn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gtlegciis.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gtjyyoqxk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gpourpaqp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gatrhbcdt.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/ghbsloyuz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gwmrafrja.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gbaqcfekl.sHtML


<!-- 参考信息 -->