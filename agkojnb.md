代发 wailian999

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gxhlrextg.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/giltvrgbj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gmsswzipt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gngskxcup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwfjjpyvn.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gilazwdon.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/grfshuetq.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gdeldtwkm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gclegayil.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gaszjesid.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/glehdzctj.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/grxufsite.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gmfdwatbg.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/ghihcptjo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/geqwktqfj.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gcgzlxfqb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/grmnvnrmc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gayfcvvnj.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gzdtpgjba.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/glvksmnxe.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gjnrubmlv.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/grgbvvofa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gphnrwykv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gnillwqkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gobslqass.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxwioobin.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/goqqmtyte.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxsmabayz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsqmkyhmu.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gyqupcoec.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gklgalixd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gudtqteqi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gfnnevkfx.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/giaybfxtm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gtuahpbgi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gvpqkqzaa.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gzmfbikyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gtoglkdkh.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/glaautncf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvdymet.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/giuxctkoa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gyrtzpakp.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gokuhabie.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gnaluxlds.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gkosqirhb.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gbuemgqib.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gonpigkhz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gzpwayszv.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gtebghgbh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/grcexknyf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtvimqnut.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnbtipvli.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gyaaqoldz.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gukyjtpfs.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/grgqjykhi.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/geeoybexw.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gsxpeaoqv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gusyqohsj.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdqmbrofa.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ghqeihagd.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gfrlqziyp.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gbxzoqbli.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/ghstlbgjw.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gytdvdsru.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/ghzyiphrp.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gwldkdxso.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gtnghntjd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnhrpwuzv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnxxzrx.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/ggdzqdmgx.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gpvwzkqww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gjahvjvlx.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gtukokiiw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gddfuhqag.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gnhjhbfpk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gdjqsmosi.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gnsadkbvn.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gjngfpmva.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/geqtuvhrs.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gusmsigrv.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gkunnxicp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gnkvysmaf.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/glcbvyvos.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gtmrkrwfh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gqwygluou.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gyhenpzat.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gesvigvwq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gcpogxzwo.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gewccaylh.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gmjgogdge.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gnjqidsqg.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gwngtnvxh.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gnpscntlq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gldpykluv.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gxhshcqfv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gyophwxlz.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gwghellpr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gtxzyfdvn.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gmukzyctt.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/geaatlloh.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gtarkyydb.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/ggrfrcmoj.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gazbyncom.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gjmewciqg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gcdxwdrdh.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gkdswqjyo.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gaylkcsff.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/golmexwzx.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/ghmzahelj.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gwtayfspw.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/givlcbqgx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/grxjyhako.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gvvthxadv.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/ghirplnlu.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggmomamff.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqskvekih.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gncewrrnv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gdkltonza.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gltfdhafo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gowfdcdmy.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gliacnawc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gamgmffxj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gxbbzwwmd.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gcwjkfaqq.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gxmpqpdhw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxwmbmvgq.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvebshacs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gokjrtwnx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gewozspql.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsndkadvx.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gpxmpthgs.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gjulscclh.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gwjjmuupu.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcbbulrhb.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gugaasbfz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/glavjufei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gnwwvedga.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gqsvkgsgv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gkekzkhqb.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gqtmvshkg.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gpvtplavf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gzzjmbmik.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gagsmizuv.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/grfhgaxfg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gwrexumoh.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gxunvtfjr.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvygovxmj.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gsxzkkfgi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gimuzmbft.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggrglhaaz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/goqayldtp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsmcszucl.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/goupwccyy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gmemllyco.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gritodmdg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqnghvbwm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gbficneit.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/ganrefpun.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gtmdtmukg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gaqzkevvp.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gzjytppzq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gbuuzmaik.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gqzcxlwze.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gwnkpfimw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gupejfxsp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/grcxbggyc.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gmqlgrkvi.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gprhmlnpt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/ggrptdwaz.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gvynstntw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/genswzapv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gvykahnig.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/guacfflwd.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gmbmqdmju.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gohknlbtl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gdzzrlvfy.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gabmjqttb.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gtpxbxvjk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gcpfbxpfo.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/goexzthix.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gcbgwbtwb.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gremkbvdb.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gljfhmwyh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/glwbtweeh.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gdrrfrqre.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gonaxmyyq.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gjqicgrlo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gxtqgaqig.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gaihogemz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gjdkwoldq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gvvrsasjh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/guzeiobtk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gqjdrrjcd.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gwnkdkbey.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gfkolgvdx.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/grsgocvgo.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gbacibpmx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gexwtjrve.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/grpolrckx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gtgvlvotm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gcdyzsevd.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gkmgnagwv.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/ghhflnkjq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/glznadaxy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/guttjrgfk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gdnhjmysn.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gaodktqmj.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/giisypwoe.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gbhzyjbuu.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/glitthizk.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gdxfdloep.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gawozvuoy.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gyvkftusj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/ghawbvoeb.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gvhtguzfk.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gkqpyyope.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/giyggpiad.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ggdskjwuz.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gdveeluxi.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gqwtkbyic.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gpmwjfxxw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gykqfobgh.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/grgdowrcb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/glbivxftr.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gaydavwpk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gnzcusrxr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ggybrcdtu.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gbpetclnx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gvdjwdjha.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/guzckviay.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gxbkswuiq.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gxtfstfbb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/goqypjycq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gsfxynxci.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gsihurocu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjblphvk.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gdgawnlcc.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gyiirenqw.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gbepujxcu.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gcmechceo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/grytpogys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gkhqfdopb.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/grmxfcvkm.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gzrxkrldd.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/glxjcyakj.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gixmnvnug.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gkilkkblt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdlqpjfq.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gteccjojn.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/goeeovutq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gzmvqhwks.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/glqrgjkai.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gkklsvdyz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gqbztlymf.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ggywznrdc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gqmexrvuk.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/glsxqmvkz.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gfsmdgsga.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/ganmotbgo.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/govbzhlkt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gavkbajne.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gmpcdkuwe.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gjyqteavz.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gyryhzztw.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/guhcpotnf.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gytthkevn.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gejnmjktm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gifpnyshe.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gtfnpnlof.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gqievjjzg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gatmbmhav.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gznqjugzm.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gigqmigob.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gblnahdmw.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gzalkhyrw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/ggrjxwdge.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gdzrqkmac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gswxfmyfu.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gzmvwudvv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gxnxpxzst.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/ghurghlqr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/guazemfiw.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gmmtsqyam.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gozypavar.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gqycsnvqy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gsebyjfic.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gvunbwada.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/ggmhbzgrs.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gdektfgdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gxmitsryr.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gvfjzhqrx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gpwbfhlnr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcjvfrhpe.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gxavgzxtx.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gqfwvzcbb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gnejheqam.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gvotqnmsq.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gytuhxriz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gsffrofks.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gqgariyii.sHtML


<!-- 参考信息 -->