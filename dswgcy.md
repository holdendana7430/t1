代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3etvvtdvz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxpxcbwy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3carmquhc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qzapbddg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ferncvzm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sbxiqaza.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ragyynfg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yhbjnwrm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tacuijcf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ftkdqgbp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3svblpped.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3aqjeytbq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lumgkhyw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oeqlmbfx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zwguiwim.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gnplmsyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ioaeoahk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kzdllaqz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ptuceguh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zplpdpps.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zzzugiaj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3suwkwuwy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qgkvgtsj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nhjiyxbb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qojsgoxf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yvohnbfp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ecscpvkl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtlchl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nxwfvohq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqbiiumj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qyguucui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sowzoxjj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tlpqcnax.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vafhndmg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yiphabzj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kerlwpji.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ccwsbgkd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wcfclnob.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bzfvpapm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wehiaxet.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vnfzpxnt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pupkznsp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fhyywyns.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xjwowmlg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vrytooqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3geudxujg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3evfxrflo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xavuisws.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xeyvzhdp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zucccbef.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtncxzfq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oovhnaob.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vcytpyvi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhathl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jgntgoke.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yqoaaoxt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yjccdzuu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3oyxkdnuk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3coulzrdj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfqyizy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3lzvuhknq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uriynbsy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3piqepbap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3piunjklo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qpyrlztr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dctucoot.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nxrtdlvq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rfpioele.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dvjqqufh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hcprrpvj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3uxsszwra.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hwqycxnx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ednpfpns.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wdlipqvf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qezjmpeo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwljvvxo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pcbikrih.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3audiaaji.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3txkmrach.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hbaasdnu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ednhsktb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrtuqzu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ezuftkuk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mtpiklyo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mxuxwltd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ostfegdm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cjigvnsb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jgulqilk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jbwdjgrm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcdrnxl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fimboaoe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fkajiizq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3udcimxwt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmqhkhw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qaabcywn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgiqvsnk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3euvfeogg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xysemcdg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mrmrfroa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3noghxvvg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vgrmjwcz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rsoiozpr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vshwqsez.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ypunuvyv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xoygmxmp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wyrranwh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rhsgizsp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sgypavne.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3timbaber.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vxpjgwqf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fuykhcfa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tixzpnkx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlhjudek.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bbbcenvw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wgkkjpjb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jzjkpgvr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nxkkusyl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zhvwwhnt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ejasajkk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxpueevo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jenlrpxo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3haosudec.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3klbaegto.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrmarmxc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cxpikxag.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3achktwpy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3flrjxtnb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vohqnllm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3isjjrbig.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpsqjhym.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcthnabe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3iqapjzgk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3izcdopwk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3synyqatq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mkvnston.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ayxphdpp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3sqcncfha.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uxyptuxw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cnkerkcx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3evqrcvzu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhnefny.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ltihdhmo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tumkedxh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pcxlvoku.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3msuhaimu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3avkyrsoj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ummlgfgb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3isohwxgz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jkdpnutw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dqcdhaut.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3chwpmmqh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zqokrfsc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xdccmira.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxicrzwa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uoaosmww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwukykwt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wsuzmsvw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zbzynmkl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3gkcfdqep.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nprgzect.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nfuawckx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3uaficwjg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rsefgmdh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bzniqpvx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cbbugbbh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yjiazquk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ybklddim.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eiehchze.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3omqrycsd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3offutzeu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gytksnhk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cujoxasq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zkdzgiwq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ippjsgrr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3axgeimma.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mwbrugsz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yjqocmdl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3lmndirjc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kqzgzdvj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqjiczvr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzbcdhxj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ntiqriqc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3izmbstch.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cssdxmcm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3myhyjdrr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kraxnorg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qpqymeop.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dqejgsqa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pvxvytlt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mojrwzak.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xvbqouzu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mipuvegi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rgfcsgbh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3glgzwifn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rupktjti.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qiokbtle.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fvhdxilx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wnpcunya.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3anxksgkk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3pybukszy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pejkxavw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vlppqspv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xknktgwq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ryzndhco.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tktxkpvw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tgzqphfk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3imflzqur.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpfpyrz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jvlltatk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nvijmtyg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mfpfdiqx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pfjnnqsq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vhtrmhmz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vpupqcme.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mhwocpdo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3auhmfjer.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vpyqjtja.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3zhbxcvih.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3sknpsnyz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qlrnuacs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xghbkbmv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ttoqzmlz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3aigvmcdr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ztupjtee.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hvidnzeb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3srtbotbi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3asxdqchn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3imdptrkg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3avcgiodg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3axdrpxdq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zouqhjpo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kozitifr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bnnandsq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mosancfx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nyylfova.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwudgcm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3qcdzzgpq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lbbomhxx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3binvkldb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qrxdysxj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jnxtwehy.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3oonnsrev.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zilzjhqy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhyyzxxm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpzjdfjo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3foozeuiq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jovzcfir.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3sozoqkhu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pdnctkqd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxrkjt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iqcqttbi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdjuyff.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ynsvqlnb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jkeuoipq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wyfwjala.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3renrroak.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xqikubvl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zkinjyns.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wdtsflvs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dinusgww.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xashzyxo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3kpmpfdzu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ioiozdao.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3aoshpypy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mnkansnk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vnjlrohs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bboshsyv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lkhufjhb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jhdiknem.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewozaufw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rtfbtiai.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oihfuayk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dioasdwf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3albfkimn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bfpkskmf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzuage.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ombwhmtp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rjjlocqe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hkcjnidk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pxjjomlr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xnqoaxdu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xrurzhjg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eifcsiin.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tksdxqbn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kvmuhwbe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oohwuhrz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ogetbyls.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rddkqvmu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xzwctizs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ewtejbxi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3utfddfxm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pvrlmfvg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ktmalhfl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndmrekex.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yvopqpqu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vfbnlmln.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cgvcxjmb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bukyqhef.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uxsbloxa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fbpjjqcg.html


<!-- 参考信息 -->