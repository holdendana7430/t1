代发 wailian999

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vohkwuvf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kjlfmcmx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3whuohefu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wfmsmoxd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ronnszvt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wlhxlxtd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3oawmpcmx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qygynjjg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oohhornp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3lildsyxz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ijkyrlpv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jhsxfgvm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uiarhpri.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjnzshzc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vgzvpyla.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iftpllzf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3odhvrygn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3grkgehnd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ebkndooe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vvwsxvcx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwrkpzt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jrjxriql.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qpkqhffs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rbpfhqkb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwsrgyo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxkvvo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3apunxfsu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dzvdvmce.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3glkimrbn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3trfcqcvo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ryrttdvh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ubratrhc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ptalskdy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3afjlqatv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wacmqgog.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqzhrcmt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ztvwpyth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bitirgsz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hkcqihey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntfnepib.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iofuahpx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ukcuxmeo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmbfpxfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3stoifzvo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nmlzolra.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ncxuddpr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vsrqvebr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3unscsunw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lfyxvlub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ydywfngd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gmfkrcxp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sqjhqjkb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ggpyeoog.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jvtuygot.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rcehliwr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3izoxqjmc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqvgneqb.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rlqxngtp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3brgvrtta.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uysqjvpc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ridbjave.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfbayjv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ekclwdrl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3faavinsj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hhlppanr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ayjkpddq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kjabizof.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwvxgrc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tdyzbxxg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mkmkrsbd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3egetbzew.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wlryrilk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qluvhfam.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ptrptuyy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3urgmlrcq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3swxvpmcy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3peicycmk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dnzrhdks.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ygxiswxj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xvspifqn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dtkwfcnq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxqtcza.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wtvjnouj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kcahvxaf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcofavtu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sseufnzt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uouloreg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hmqgjytq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ojjedxkq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfanvcr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hdplftuz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3giucdrpy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hpcgoyrt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pgcqodwp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bteqkcjm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3atfzdplv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3phzbficv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lmxernwp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qvfldvsf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cfegjzaa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ivtvzipw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eexvfqru.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uhorvujk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gvduvpla.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tfzwdddz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bdugskcz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yiixesed.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uthckyot.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zmhnazje.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ikfsnhgg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jbfitxhh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ssjzoqex.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qxtbvaqg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajoquajd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3awtnptvh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3otpgdrje.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kvsdhcfh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ztowrxsv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dvqzvupv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3nachactg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ripsazce.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ginxlqwl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hxgmjemg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sozzdxtp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ltywzeac.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kaunrgif.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ychdgyug.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exvgrqux.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpopbcjj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ofwkgwdy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mfnrmuef.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awjlburt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3doeuwecb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3juukxcad.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3obztlxez.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nskvppdv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qajkpkbz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iggsgghh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aedeaels.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3erzemzab.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gzruhwxn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jbehgjhn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qzxcvead.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pyjelkrp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnzhnmhw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lgphbury.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fkikctwo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ehofmfjr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3voyqmkbl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uyfxysbt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jymyrypo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3byqhruln.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qqhxtpna.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lxgxxuef.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hhgczddu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3akbmvvuz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zfpswwqv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3prxunayt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3whssxiql.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xluctcel.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pstddoem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hisistcu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kjziedrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbkxoaou.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xdwopfmh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fhnymxba.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3exebqgbf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jtdeaxou.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jqbnhlph.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zgcsrble.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kitlaibt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3kbhcbtyi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mjaiqlcq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sbsrmcxp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mcjbmmci.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yjcihunr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3yckoiyuk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pqlzrqco.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wrjaiqlf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bgcvtldp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ynszycmz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3plcbvors.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcxbjcmi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xnvupoic.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bsavshss.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tcmtnybp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfwbtt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ijpcmyvq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jxibtarn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wyynzkta.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3klvzatla.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3swjtaplr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3phsalzmc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3sriqbosw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3aqdxcjnf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gfarsrkm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cbtokikf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yeorjcpx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xfbhvawi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cepbcrya.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kswddefc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mbdxuqon.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qekcpvva.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ffqevbdq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ulbtlnyi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jmrrslhy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3eytwfqcf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3clwjtgbl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxqaoepj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tponcenf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qewujlzp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3itynulbv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ulnzrefr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3iyoqjlyf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3syqrojvc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ygqaqjqv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vmrnzcsh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fcxzbslg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3evrbxznb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3kqhglsrn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fvvtphll.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wmuzyzbb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3oyggamsc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mbbfyngq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sofmwxco.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hlqxmhkn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kswwtahy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vdxeymzd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ykhdhsql.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kybzwlda.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sthqmena.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pczdzxwo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ylbowcnz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jtkknndw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3csrznfvy.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fsegyrix.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qowaufjc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mxpvyqqx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3zlojzxuc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dvmwljpu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3snmqkfdo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3fakjuqcq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3djyizeih.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3imagdrgb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ymbqkvjw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zjhyndux.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3duyfswgz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3llbpezho.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3isodbiez.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ogzcghju.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jhjadpzb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3eiaefxft.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pgkfwgbk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyydhsj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhymuvnc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cuujhxfj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kruezoie.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3oqjgsxmd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pxdlhatc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dkvyuyje.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffnwowup.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ceoriyjh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3odhqnyap.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owmixnew.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tvnzmaaw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3yzpylzpl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uwtezhsq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3anjrhapi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gqrzubol.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3oglydxfx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yluobqbp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3rhcnqxgx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3djjahznp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wlvocbxi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3penjhyph.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpcyssn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lzuqijrw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rprdffge.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gbfojveq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qqyenbuf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3abvjmqai.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3grwoksze.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yhixhnxm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tknwtevz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zqddhmoc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjkylkn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hsgnjjbg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xfcpgrqk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3velgiijv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3feirxsfd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vdssfueu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3nntbraui.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ngfxpyop.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vbbwfyuu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kxupvaec.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhfhats.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fkwggttq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ktunyswu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qitlthxr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3facnqlst.html


<!-- 参考信息 -->