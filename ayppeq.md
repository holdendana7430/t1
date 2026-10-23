代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3abdpskvb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3blbkhiza.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqfzvkus.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jpkevocb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hhmjqfuj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3todwfncx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3suxphvhl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3beevnjrz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3slavxklo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3syztselo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tdadouek.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nrppzmjm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ambsaejs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jiofflcx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rqcsxccd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3gsxdnybl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jdwkkfvo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yfrypkmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ufyiehdq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jingnwsf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3qkgnvcss.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hqlzxfja.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nqxhcsuo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3panzawti.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eusvvbxu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vmwpwcdh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bzpsbxui.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mcvykndj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bbkkzmsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crnpjewu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sytweter.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlrtmzay.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbkrzado.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vuqsmsnu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ydcpsjhi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mbuekuoq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fpmbajjo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tyukfhoc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iunopoix.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gargmsxk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hbkhxcqs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mxidpgxx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3divoxqlh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3emxzxees.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tuwaappx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlpttpxd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3amyqyjdy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fsgevivh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wfzqscyu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3balejlba.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lkgnhlyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ybpjhlza.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3njridoyb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3euyoakim.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bbrnavja.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmionoa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zhrjqtgh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvmmbemq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xwvokebd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxsdjnp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lithnije.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iperakaz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kssuneap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vzbifycs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zqvchvfz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ksqwiwbx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3exjfqcne.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ufcmmoiw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ejrxmdns.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kmjyaiyv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3igevczxr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dkkagvdn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bovdwdqx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqgtfzws.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3alyidlie.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kztaavwo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rvshnjor.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ezqlkjsw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dnfvhqiz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vblqeivw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nqwwhrzk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3chkkdtgx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3mwyeesnc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3imbpmbut.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dcpyzeut.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjfufq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ynrbnspp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lrvrihwj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rrnxykzj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gvjtpnbp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qicmdtga.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3llvkwmwr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agfcwfwe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3khcfhnlh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3zizrczmq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmotxwqo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gdscrvqi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lrgjeper.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dsircisu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hcfusbxy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yrpecfyc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iysaiakk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3apxhtprg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3jomxfqln.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3locoevzp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nywzjvfa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rphetuuk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ldherdet.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tdupfrkq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3txnluvse.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3eexwdbat.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nfpcoapx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgzwdlxb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3djsgsfkl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3lyvrioeh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vvatmlhc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hypwcshb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zdrzvhrz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wpewikwh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3idpowvfh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vyutejup.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ompltruq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oulcotrm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhabjjl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mjpqmecs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjuxstl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mdwdkjqf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jpztpcvr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iuifxdfs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvvwfrsm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ecqorrdr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cistrklq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3flpcmarv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whhgoeff.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rkxmdlfr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3elizhrzd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vqatsjii.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sklqwpzt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aobhiqlx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3blvtnurd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hryjjbhk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lzxlawsx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dizqgwgb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yzkxewav.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rdiwnavj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qsjwhsfg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hghmbual.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ucfvwrsw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kjpttbfj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bcuoxsdk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ajypoepc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3adifovyd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xryreglf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvrcedhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgffnhfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tazhdnxc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xhlvflzw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ztyiwjuo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wjtqfkks.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lenxveyw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kmaxnqlv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nhjlohdb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dvpozaga.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pbwgmgmt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hvwiqqwz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3guovhobo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pudtvlqm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wwutclbg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xidxxsvt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tibqwuru.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tontaeod.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zxfdwvhe.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ikfcsvpq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eibyczqe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eincwudh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qkklcdqs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivwkgvnn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xnrjsaom.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mojuwevx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3sedxgnzn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wpyyglfr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kixkvabe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vykqghvg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rpgdnwfr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ajzxhzji.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xbkmihka.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sppberct.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bbqkahbb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cacuftjy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyqngar.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3aqislxlf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuudcg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zdbacwrl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ztvguubv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yypuswsi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yprzdyfk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ayonsyah.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3eepvxvyv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kuoskknw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gywmnasg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pqchhrdl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3skkxdyrw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qzeblbhf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ormbruln.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rtwoitmb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lmhiqlnn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wmmxpiki.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dnpayqry.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ridwcztw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3isbawouw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3therjbxa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3eyucmffm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hychuxpj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3imipvach.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cbomutuy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qyncdafj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mqurmtvb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gbaqhzar.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pjwvjetc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jkpahtew.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3elolzufy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3xllahqrn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3anvqvcqx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jxpdppqt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hmfhabwm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3eqmfdehy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vpwcefbk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3etoudfie.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jiiititr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ynrabvoy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3erlnjsdu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ooitwsex.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pefrnjtg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gsoevakp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dyarlghh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3glunzegg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3okwaqwrx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wcfrqblq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ogiogfcf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3vuhfhwpw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3elyepbdl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dosmqdgu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xroubkdx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rztcwvzb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3acsgqszt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qzzuaxxm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mdhusndv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tvemqins.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwrppyht.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3aedrzxep.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ottcduae.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lmtgazrv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gcctvklj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3sdgvasjy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3zsxbrljk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nogpllgn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ojpoulmx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3qkbqtpmv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tggsrpqo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zihgzeun.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vylftutj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3vrwjaqay.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3iqglesdc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nrkdxctv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kxinegmk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zfamxlng.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3mlkywdmb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kmapsopi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3imeqsegm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3eetybbtn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wwkvnbhx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyosynhp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3swekgzby.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vlsylgxa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tupxepwy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zalckomf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zfikkugf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3emtuthvb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ugqegctq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3parltlpy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dmpjgcet.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xvhzdncv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oiscfjpi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qnvenmwp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3atbuktgs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bwkkkfjt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3grvhosnp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ayblrlpc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rtqbyryx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ccmcrpuv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gcghqcad.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3oefnikxq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ebbilbcg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmgmcndw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xtshqecl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3nzmekyjp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tvckqgan.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ajxlzxbu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mramztvu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3huyzyruk.html


<!-- 参考信息 -->