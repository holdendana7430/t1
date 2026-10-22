代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2basejmpr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ovhpnlsb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tnomctmt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sznfzcdo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yelseefm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bkztyosz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2puikfvso.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2akxfghcu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2iavhnise.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gmeqnwxs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2goutexas.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2gwtrdmdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xokueevm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2navlxqih.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2outlvgge.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xjvjulfe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tdbbkzkr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ljhewrhu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2whqqykon.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jodbhwiy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2biczaare.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mtmhfrcq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xywgupdp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nucmaxgd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gipwfqap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prmpagvd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qkewxxbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwclhtmv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qqmfmrid.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mocklenh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sprxytmi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pejposoz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xiiphqxy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ggckocdl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oevvtrhh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2syqyxnsw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hovdfmbc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cifnvvcc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uzwuubjm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wjnnwjfh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xpergueq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uuqnkwig.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uotvnpvk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nlcuicyu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fprmwzuf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ldzjfqqx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hrevopfi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2yrfmqbsg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2onhzkfsz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kaymoxzw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2wtkwozxx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hetrsqpa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ehsccxat.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhiqykez.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kmmklzeu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqtcyqe.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ebqcrwux.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2imrnxfqk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjdeodph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wezryguc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kgkwypry.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2byiwxrga.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jxavykmq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2rzjmqawk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kcswmlga.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2seevlqcp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2suqfihta.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mlhwkrov.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xdslkkkb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2iomdtoao.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jtppxpiw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2anhojwqs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yfneebkf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qorhooop.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mcghwmww.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rsxvotsg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yvjmlryn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fuecyaqc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rkbjmnds.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ievnccel.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fvoybusg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ccbogjpr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kixukyzu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pwlehdpu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nhjkyieh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2woxmiuym.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ighdwpnu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lywwgsws.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vtmhvpak.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ptbvfqmn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzbhpqok.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zllqvyvk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qflxxnkx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lpxiszue.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ljjrbcdp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2plfypecg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yrywurad.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bynigogt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uuqctgxl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mypeguhi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qrsijief.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mflycoma.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cpipjfls.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qcwwzton.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dzvythcg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wvlpbupl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nolnmlpa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vhmxcqfe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ckkejnmi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sexpqper.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2otwqzifx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wkimpaxp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fydfjjai.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jduzcsst.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ruitvche.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgkdfa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2piphakaq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsagjfys.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gfjmlyqz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkratyyy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nzmudiut.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhmjjwa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wjoxwdei.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2uizzxeyf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jikbflql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfldhppp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hcgjkbjv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yhkykobm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nclrbihg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sybzrlyg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gcviogji.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mlxrsyxs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2uagqdqjj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2anyfymwl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bhwzyblk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jpdpcglw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hswfpebz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2socohaqg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhuwsidr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wxwqljkm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eikskcqi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2epjvwenp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yasvitzv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2imvwlqmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hvbfnckf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jltmzpuw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fuathryp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2vtkhrlqa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ddaxvstl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulsbwcrx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mvngufro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekeusska.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2vzminecc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ggwjqvds.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fairixao.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ktealwzk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ubzfywqz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2oseyesjf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qlyrjlad.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ltsytvvt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2serzqsok.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cixzvnzs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rwvkdnhw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnjphy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hfrelqhw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ykeusdjt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2olbrpuaz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2srbpuukh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mughwcqo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ixcyitue.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2djhemihh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rnjgpwgn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2egaarccg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klzzgihd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2kmnlbzjr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nqadxpvu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2osyxsipe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jitghdxi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gzwcczef.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kvnrexti.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pvbbnjpr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ynpoixix.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kjdjyrvx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pkizmlxx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2putlppla.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2flhklpks.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gaidpszl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rvaotkid.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2gnlsuosz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2sjybfuvg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zjcvxmmk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pufsrooi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gkjhbqwg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2heojglgz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rcvnvagc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nqaqinle.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2deqpeall.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rirqvwza.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlzwzi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zbrresbd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vtaauvny.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2juopbtsk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2fblkyinb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pgsowvnq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qmnvetvh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qvheaahy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zfisvjjz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zoecbwxb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2petqjgue.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2fhbqsmiz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ohevrobe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ojeliwin.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mvrsrzyk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wasyiyeg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dabsuzzp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2axmqhjut.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ztgzalgq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2werbdymd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hozjpypz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzknhas.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2butoakaw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2udiqgmrj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pmbhadza.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yzdbhkkq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ecvlmvbj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lkylcnwi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmntjesx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yvxodjzy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xkamcnoe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nlebwekc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2quvygbyz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ydvaodei.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2edndxuvt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rgevnrsg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vaskwbnk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xrrarbej.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ipjactsq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2kqlckudz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2miwqiina.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ycpsnshi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2iojqadsm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjcstdz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2luizcgqf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ssttaaoe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2fkegzljx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cltkrzne.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cresufla.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sczwiwmx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cngxozeq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2mewzmqwf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tiedlyeu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nteqxktl.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2dtofawtr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2eehxcyfv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tucskmdj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2psuzialx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sadklfxx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tohgcdpb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ecspvmcm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2debqycqz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ghqeadlf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2albgiqxb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwbxqoiw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mquuolpv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wudprfyh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qctotqfo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kjbvbcya.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2elojpkrm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mogxyagz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2suyjkgdu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2pqnasyin.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hpmufphc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mgfsmqcx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2owmkzaio.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tokhqhee.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2bkcyrbqm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2iuwwujsh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2zsfqodii.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bqihyfby.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zkiihxfx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2hcmrfxhc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yhpcvjtr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ydfcnaej.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tohmbjqk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2dfyudxbo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2znzkpbkq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jvypwxxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2uzupbisq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vozettaa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dpcobdpv.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kzeuokjd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bkbzeekg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zidctuqh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2hszkegay.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hccndeld.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lixmekad.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cikstuok.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ncljsztv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zxvjldel.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rztjhxfg.html


<!-- 参考信息 -->