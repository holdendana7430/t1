代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gfrrujon.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gmwpfcep.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xnbjurte.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kushslpy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sgtuvtzf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xhbwsgmj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hyfzujfb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rsccbxvk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ojmmumik.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gbdszuxc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fpendiig.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xlcqhjxg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rwgfuftm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fjxrvwie.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zezebpsp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ercwvajo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3uuunircf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3acmsimod.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3luwcraxx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jdhlwyes.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbcfgac.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3opuoorfh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ereadocy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jqldmqsr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3axitwxtx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zkqiglwx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tcoxlxov.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rqtvqbxu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjidqyfc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mrycuili.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3begiurfj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fcsgcfoz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vauebboz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfsejqgc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3udhcouao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbrktjbp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uzqndrmt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zgyrvste.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zbtmcmja.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ppyrabwc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vildhcje.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jegydmkz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aqrvaicy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wogywwib.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sszyvwcg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hjzjltza.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kqvwdsyn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vdzuqplf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hsswkncw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmvezqhf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aeroturi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3olbjppeb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fnkmgiqw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cyggourg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3nvhknkzd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uxwyjzpb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zihmxdxb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rccmdgib.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tzhuqviv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfgcmky.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aaivyfbh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdbxtpdj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yqkuzyqk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dvbipxkx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ljyzzfnu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qngjwqpn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ddvpmqkk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3biizbalu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3prxxngni.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lttyorbh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nhywztxo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rmbqsemd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lhxdsrlx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3plwovglt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zfrjdpkr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3utxtgzlf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3svpeyjqr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpvimxgw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3quqycnxn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbzichfb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nhudeqwr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3iciilnzv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3agzdugfr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jnwyetor.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zhvddraw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tjizgnvq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fcvjbwdp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ocyvnryx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vtdexkmj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxslxzrk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fufzgzuj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjbprkv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3izgnwmtj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lomomfnv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cudthkke.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3myjanhxl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3agmbvylr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3urbtmnxs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tphokvna.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rkemewsq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wkgctrfo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lfrbhxjb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3engsmvis.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vgsmccif.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gxhcnmov.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uyarjlzj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oehnrjho.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gmvzmoho.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hzrhuaid.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pecmvwhg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3srmibyvt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tgjjzead.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gksplczg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3saeqpidh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tjorrdom.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3obkzwnhz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3obwxsnka.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qfiqeosx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3emubgnzn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3baqgrquo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dksmqjod.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3pbmopfvk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sdldocpn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jvlelpkj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zpxowpsc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfuoxlnx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3plhhyzfg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3odpzwmhf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tupougqy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3yvoufhjz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wgoasuxt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qjcwhfko.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxcdoolf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hstnpzgl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfrnhazs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3htlaycmn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzscpsur.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ervszktq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kgayohib.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lynsylna.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cbcgvfsn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kbycxfbr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cbomjedl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfdwxv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bocfomrm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3guzmkoss.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tjlxashu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tcyqlqcn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mynyrcju.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xznxixem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pscujnpe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ahedmmjw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lkpgobsx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwjcwzwj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dluqurhm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nqsjeyyz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ejfqpvra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mapgwcol.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aemzdeel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsaqxcon.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3duwxjgxj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sckehaxd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ozfwzbqs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dalojjvq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gfvurqyh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hsaptxhd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sxtrnmlb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uizxraql.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xoxhykmb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ehkqwsmf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3wweorypv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oikxxpfk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3iuzioyax.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wffrqqnw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3axzjwpob.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ambvjlqf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3itpkomlx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwemwdu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ghulgxov.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3yhzkklky.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qisgqeza.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ioyyxqid.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rqjhmlja.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3murfands.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwbvhg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yzsqmmpk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3viuzmglf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gyyondxm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wstnfbti.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mqfbzass.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3twqdpgus.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uppcewdx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpklxc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3akumezen.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tqfmukvs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3stllarqv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3snpgkjez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3udagdpwp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3onbzjzyj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hbnpzakw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3aslntflw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3swfoepgd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gyonpfhl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3cktpcypv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3eeknxkaj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3osnfpynw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tibmtipg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bctysekb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qjqfflvj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jhizeona.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pybsdtwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hiekyuun.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wqazzyzv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wntspicj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sboiscaq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kbjlmjjm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mqcilnvj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vemhjlft.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qragrttq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hshydlqi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ksswemqa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vaszoovx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ocecewtg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ysqrazav.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cfbuhmbs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mtajiwer.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fpfnfgtv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3offosyer.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vdyvponi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tgquumvw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qikqqpvx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qbaxekdx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3liysnctr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mseqnbxw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fcyxspny.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jpbahwei.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3clibmczf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3grkpbwxy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3nnvvrfrk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vogymhgi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ygufrbaw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3qvwgsiuj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3oltddfqi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3kosimdyi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3edxuccbe.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3xmhrhtxk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hpbqiipe.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uydguonb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ofmomxgs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qmruqxnx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uwapmhmt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3epdwkedb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3iqvseqbn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mfmjtxnq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vpiwczlj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrfpybip.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcacciye.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3laelvtug.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3evxckwsg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dngmhijr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3egtfdftw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xftxfirz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dhpmbeva.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wmhhonop.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3spkabcsu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ibfunakw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hiuaomyq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3sduzhyjr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wzzcnksw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ebyzenvf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zqshqwql.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oqkqqqme.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vtzxltrs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsbczobq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3coctpaqo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wcpzijxx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ocrthepr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ykhwfptj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xaxuuoon.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ygetamho.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tosbynpn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xflfovqv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhncuhqv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3glcfksog.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gjxolstg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zoamjpqt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jnxghftt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3micytrth.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xqjjjort.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jspudfpo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ezpqmnep.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tmkjgmyb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3gewvjbup.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ioatwkam.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dumkcwrt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eallrdtx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qhodavus.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3stqevlao.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lccvnoas.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oqxrrxmn.html


<!-- 参考信息 -->