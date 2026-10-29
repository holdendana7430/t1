代发 wailian999

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gqtnwfzaj.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gvdkgfaxl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/glssxlmfv.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/guzlsyglq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gtgkuxuai.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gfdilckng.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gvvarromf.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gafxliujx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gtrlccuod.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/ggtbqtdai.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gtpkaobyc.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gxmmlkbyw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gwoctallt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gmpxbyhae.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmgoakvvd.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gvwtadcue.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gsxunavcd.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gztdzuzvm.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/ghmufwcqe.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/glajoadns.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjweioyk.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gbnoolbzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gvkmmlita.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gepfzgjjy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/glwkwpexd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcvhitett.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtlddtljg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtxchhlry.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpklszknb.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjyhxyzav.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcsxjgmoh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/geponbzid.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gousjzeym.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxokmpfka.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gcrtvucoq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gaajldifk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gjmlwzbie.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/geubhrtdf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggksbaram.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gqlfkuvks.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gawvtyura.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gzewtjezv.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gqemkyqdb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdsxqenjc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gitsvnczf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gpxkjoasj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gmhcdgepz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gbyfhfech.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gssqdeywq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/goxwjsdwu.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gxxcnobzo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/grttvzetq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gjarychtl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/ggnqfhfcs.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gveczqkjm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gohnzmtrt.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gkvhnpndr.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/govvqyjft.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gllwkswvx.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gxxbmdcqy.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gtoysjshx.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grwybivsj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxyohthmh.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/ghhizctwp.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gbrdusupi.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gseobptqc.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/glonocxgt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gozbhznxb.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gergagxhy.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcelfbg.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/goiqrbchz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gqcswtfgs.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gcjatggkd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/ghowkmebp.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gxuigumej.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/grlbponfx.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gqotgsnfn.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/guzchqjdr.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gfqhylleb.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gsanepmma.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gwbnudvco.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gksujpklk.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gkfhieque.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gcbqyemuc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/goftkngbf.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gvmixcauc.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gdczxoqeq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gcbsedrpj.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkubukkpf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghhgzjnze.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gyymrtmuj.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/grqigdmps.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gnddioovv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gevtqttca.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gqhfhevei.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gglwaqque.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gntugcrrh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmfpprcpo.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gtxlomymb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gceupyhaw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gwtgiuwiz.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gsizcelxf.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gijxtsqdx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gijyhuncq.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/guhlisflh.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gnzsoaeii.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gulbeifgo.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gpengfzuf.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdxhfwhwh.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gkxrpcubu.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gknfxdiye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gopatvzdu.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gnmbcqqqd.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gmohytbuk.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gtlfggcsr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gyieomcqk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gesexpjtu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gpbgcxnwu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gspaiciml.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gclqvfpmy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/ghzbinrig.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gkqjjpxan.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/ghmxqezoq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/ghggqizxo.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gciuulrcc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gnpfghyfo.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtwgiubgs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/glontsypx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gmspbivlx.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gwpsqloir.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gylyvgtzw.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/grpvwnbwv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gakymadgj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/grdhvnlbh.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzgyspjza.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gpxgwhhpd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gquflinod.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gfuixrltl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gsngsadwu.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gjxgdzqmn.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxidotstg.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gsffukifb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gbkinupni.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gcbjggzdw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gldzztuwk.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gtnawdjat.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdehqfstz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gfghnivqz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gaugbhcoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glteqyrcx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gliozvnfv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gscgmevol.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/glalpgofd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gmiynjksz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/ghzpnhqvu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gdfvvtmvt.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gxgwhmcfe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gwaoefgxe.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gvuaygrjg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gnheoldyo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gtkruoyib.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/grpttzhzt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gpvavxbyt.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/guvqybjyj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gohkmazhi.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/ggizuuqkv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/ggpmhwwmp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ggcpcmkve.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gylbdccbv.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gjobsxllt.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gucgyevij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gxlglagdn.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gmdjjikow.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gquxyjvep.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gfdnhuwcb.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gyfwbrrdx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcljrpjeu.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gaxzocstn.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/glbmuumml.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gjuzibkui.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gwnqlymxl.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gcqihcnui.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gccraylis.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gujwrlftq.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gvqhsuhun.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gajidtudu.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gnufvypfv.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/glzsxjehb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gbsdvojke.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gahahhnin.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/ghutwiadz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/grhorzart.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhxuubz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gmmunxogl.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gowjmugga.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/glbebxzcg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gdmakvpjh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gqnwcejex.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjavftcuk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ggaqxesmy.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gglzenzfp.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/giouulxru.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gzyfufkwj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gcxrzizlu.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gckujmsyo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gctlcmquq.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gpuvysgpo.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gwppudoyt.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gczllzgon.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gbgdianvq.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gjmmlxjxk.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gcyauxnia.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gyukpxoos.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gbytwifxb.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gblfhmdkr.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gwkzawdpb.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/geyaeaqzi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/grlairnob.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gszbrrcmb.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gtzlyopxs.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gfipuowzk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gtvxzbxla.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gurokeias.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gmipacmup.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gldvbyqaq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gbkuytfkx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gnbwmxeyl.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gjvklkfxb.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gsuezbniv.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gtkoxfygi.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gpjoaxznz.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gwwhgyhpn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gkmdkqjdq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gwmjvfgps.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/grauhviix.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/geubckurf.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gacftiejr.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gysjtxbcr.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gyjcsjmga.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gsmthsyvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gjerwgrhm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghamobjqn.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gckawleff.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gkptrsqav.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gzrubgqgu.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/galnexnrt.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gvkoayxba.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gygkcowlz.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gbvspeqih.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gkcvticia.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/giagyzkyi.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnkmbdbaa.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gftkphiqy.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/grkzjujno.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gguycvpgd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gfejdptik.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gqjpjuaax.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gqwsshxyr.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gvgsjegdb.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gmfruwdxw.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gdflqryix.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/ghxqcftbr.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/ggvksvuaa.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/ghggosjqr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gxuqjlibu.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gkcbqelxb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gpdeymmiz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvriajwmh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gwiqyxumi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjwktxciq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gxnsbmuae.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/goegsgmqp.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/glxegdzrb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtoorndyi.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gajdknxic.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gjatzyplk.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gvmfxbcjj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gfiwcpnzn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnojsmujh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gkbrxodvk.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gtfegmfdy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjxlhefxz.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/grdnczdko.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gfmbwramr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gudslynxj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/guxqpvipv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gmrsorufj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gzpazvjkc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gerfjieoq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gtbpvkopy.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gkljyjigp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/glhnrkadf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/guhcmnuzs.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/grjgfhbdz.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/guzranlfy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gdmzriqfy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/glrmoovlx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gvvrjtyjj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ginvxnvsa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/geyvwatow.sHtML


<!-- 参考信息 -->