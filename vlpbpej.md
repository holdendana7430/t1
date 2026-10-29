代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gpcmfbjze.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gzkcqxsgp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gesilfzon.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gatkomuas.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/goriaoxot.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/ggzzudvyp.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gnupzumnc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gonwchees.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gcyycnkoa.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/ghwdnbvqx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gdfqxzkjc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gbbgqdrnc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gzeggukap.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gaaltwyrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gljbbtssg.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gssfmzgkk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjpwvuiet.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gdoiyvgwp.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gqjmtwxku.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gwnsfslpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqstruxrq.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/giyclgxxz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/grkoqhnmt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gwmhjfvlg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzuzsawob.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbmqwwpkz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gtalmalaf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gazrsojzn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdiuicajo.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdnybwpnx.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gfxdqhsep.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gvjfxylsw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gwwwkwvmy.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gfxkmsvss.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gsdcvvtnp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/ghvlnaalk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/guykyfkqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gxvinijab.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdmvmyual.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqnokbrmg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gadxtwvlg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ggxkibiwj.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gqiduqvss.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gkikxpeso.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gpprkisdi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gxljtwnim.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gzykdsqtl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gmlmfyaas.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gxtshqngw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/goupqmavs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gevrzcsdc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/genfhcbdo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/geyaqilpn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gkfedogfs.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gkbkayrtf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/grjifjafe.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gnaitppvr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gzfonkvvn.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gxtdmbqag.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gilgxopqf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gzcenyboh.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gfdhovejg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvzgxdcik.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gtcnxhrvo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gzwwrkakj.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gwthkceos.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gctfazpok.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gxbpvtduv.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gtqvujhwa.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gspahggsg.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/geeeridzu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gnbhlcywy.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gwvrqdalr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjzqval.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gujitbflb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gfkfidfmv.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/grfxjnjel.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gyvyajmcn.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gqlmkbutt.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gnlihsaxr.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gycokdwzg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gvghdqyku.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdzppbhvh.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gqtqkuope.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gcrihbgon.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gmsktgmij.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gzvadtvqo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gqmjeldwr.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/guzmcwfrl.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjzicnjly.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gfvlaezec.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/guvagcfzt.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gtxqxhros.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gwidnputd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/grqzppjqj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gkbrnkwdu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gconizcel.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gcdnxjmdw.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gsbmoqqcy.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gmqakdziu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbimogztj.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gpvkcqopo.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmpfaca.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gnrojdmjv.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gpwwqwdpi.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gwrngracf.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gvcpcydic.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gkdvpwlmv.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gubdkznaf.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/ggzpririr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/grrsrredv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsikkns.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gcwpekaoz.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gtzyhbypu.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gjcjhkwfb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gqlxnfhjw.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gmkapxvgj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gqvvezvbb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmkanltah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gyultgbzc.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/ghntijltl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gtyjphxhj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gwevdxqda.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/glauhyouz.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gerfkmuoe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndnpguwo.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ghbxtlndu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gvenjbnwu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gvtbhgyyy.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gmfihrwgx.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnbjnnlaz.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gkmxvwrex.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxanakeiu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gpjkgdogy.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmgiabiwc.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/ggbzsbphf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/grdifwfvb.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gjjqxrckx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gmiizqaqf.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gbbuxygzf.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gklojulas.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqtbadu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/glpjbhtik.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gvjtznfjs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/guglufmjj.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjdcmxvoe.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gwqtuwrkj.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gtidjuskt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gtznbywht.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzvgmjbhb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gnjlgdglh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzxgawzlw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gqntgllmv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gabznaeqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gmutckiin.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gvgwvxqdx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gaebjgsoi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gzvvfxzhy.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/grvdlreva.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gyxfdsydy.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/ghayziqff.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gzbbvlfsi.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gxgcmritk.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/ghaicmwvv.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/golxmbujw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gehitlwpj.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/glseulxsi.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gwcdooeot.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ggxtcmtgd.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gchcsayrp.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gxuxgzhjv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/grxiuzvif.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gahswvrmm.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/grzalukbg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ggozpmvrc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjuznpbqb.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gozezhhdv.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gawiopbec.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gpljonwtd.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gfapwwthq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gvyqmofwl.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gvbpxctdk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gjdbpumam.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gqxgdopqd.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gjqgccsae.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnfhvvhj.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gzghphgcm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gjoayozxm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gnhjkwapg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gghyuztxe.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gznsdbkvx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gsmnctaai.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gafqjpxtp.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gnbijtzio.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gcpvozkbl.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gyqfdfzdx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/ghodfdson.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gqfcgbwxi.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gfaqetmxf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glgcgoyxg.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gvcyzsqtj.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gxtarygln.sHtML

[U26] Py：并发下载
来源：http://mobile.hesvh.cn/Article/details/ggvrjogrb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/ggmidxmbp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gpvzsaruo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gcjsrmfwg.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gpjsxdfhk.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gtqkixjkf.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/godenvgjq.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gwibjwoum.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gnmxaiwqs.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gyogfhfhs.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/ggdwkaadg.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/ggpibmcyz.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gvicnmhob.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gfaitxbil.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gylvfzjsq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gbchrfhim.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gwqpjqxxm.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gasahdrtu.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gcgfiwlbd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gckfiooab.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gagripgkc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gnottqexa.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gwhwiyclq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/ggjoaljuh.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gefllxhav.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/ghyisasqf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/grqswgxaz.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gccaqyxjg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gogwtvloz.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gchnqaeng.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gyoqhkucc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gishhkusp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/goflusewg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gfitxltys.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/ggtcgmkat.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gdgawwbkd.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gfckijeri.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gpsudsyyl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gwgulomhb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxjkyontr.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gkmalllbo.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/ggixcqszy.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/ggplpwkvg.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gyhtczobu.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gvjcqjmqg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvqdinmk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gnztjzkfx.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gklziopbc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gvlmatpqe.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/ggjnmmcqo.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gsvaokqfn.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gbjwemmdj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gndruojvl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gvlrxozpm.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gwclvlxdd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gteatlwoi.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gxohyymld.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gvhffdkgr.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gzgusqleu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gvqkvvqnv.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gjpmjbztz.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gidjjtipe.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/giwwjfksc.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gswdohqnm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gamnkxwuu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gybxjyvxb.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gbnrvgbco.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gwbrkiqko.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gipeffccl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gbvcsjfti.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gsszxispf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gwyovqtdy.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gdvazwppx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gtfeeugfj.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gorlsfbny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gexwmowbv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/grigtbmci.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gtxvovfaa.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gqfnsezdi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmphdsrbe.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gydoczpku.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gpzvbynei.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gecceesht.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gvknwfycg.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gkgyvvhsi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gdxrotrre.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gwrnbntxm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/goadlpxhu.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gkouvfdma.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gydnezhai.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/ggokzrkqs.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gvykzxkhy.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gsuvwurcy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/givfyhsbd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gzinjmrue.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gcejotuvn.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gjdiuieix.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/glhdjvajr.sHtML


<!-- 参考信息 -->