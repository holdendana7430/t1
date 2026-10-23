代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqrcvcc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3irnokoye.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zckimmnj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cxcijfuw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ogrcqizc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ffzxkzij.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3igpuoamv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eloqtfjl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kgnswjuj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wfffvhzw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fmmooiux.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mnmvvtfv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qzblbfvb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mfjbboeq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3saupbxfb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hsposyvk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogtzzwuz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xbcojkkh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3trmaejdl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dmxslrbo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmwtsno.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yiodzfki.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lfgukdny.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sfouaijv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khzjkocg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxxojzha.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gsmfrxtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxaowfwi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sajiausw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3txdbhbfo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ghylebzx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hgsxpczp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3eontevmq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vouwoffh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3upfnknzs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xfofomyz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nxyrilxj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jscqtjry.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dhgkzguc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jtnvlbkw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kdotrkxt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3icdivtxy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fsaqzluu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3anvxgacy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jeqxwljm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3blgfhidt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aqaibrcd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uvfyxvwg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nuqsktii.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ejxerjnp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3olmstwzu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lvqtceld.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bksjpdau.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxwpqcz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3osqmxwlp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mxmrsiak.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vumfidcy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pabrljhp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nefkgxsq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tjfpomsn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lcbgqgyg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3fkpfzzuj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nydhvdoo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3srloxzew.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ozdpilkc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mzwjxjfi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3drgzglvw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ggxqxdkj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qmhqzlth.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jvdhjdyk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tftfxsny.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tkuqgckj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3exizhxoi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uhxftbwi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ekcrxmsk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhjtqboh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wqkvcwjq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ugnusnna.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3yncfehoe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eqhwudam.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ejkavwue.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzyaiphr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nrmvkzub.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vbxzgiqs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3snrnjgdl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ukcztmsp.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ddjqiiwl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ztcrkbik.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdmdximr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dhuljzom.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ylokaqqu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kgmihlkz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hvltscbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3uztvffyk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zlydlhcj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vxlgwekq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3sdvmxjfi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fhlmmwte.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqndopzs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xzylblrj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3llxurqtq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3olkzrfxu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3inxfrzbs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3highzyww.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gajxowco.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oqxqxgfl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rkmumbbd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3annrmeqh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3clsdzlxq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mwllbzld.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3odworpfe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fdgbhanz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jnmjdzqn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xakdgtni.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bwcquskq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arhbccgg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rsjektnu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcwkpvif.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vhzvkhgo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jukfzodm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gkukkucn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxsccint.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pgdutixd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cixnjfbm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwiubkog.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbixdcxt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xinhyxtk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zjgwsjgv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iqdbyucd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uljrwbrd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3prkkfbvg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfuzwvgz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hpaabtzb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3notptldw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mldrdzfp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cfoohmil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzugtmnj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zyvolciz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hrppzaag.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3lucqwqhe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3njeklvpo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jgbyevoq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3foarxpvx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3awilglmm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3tbcsviny.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3czdqhrqx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3irkigxtu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3suztoitb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tydxbarm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xucnvsus.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jqtacdrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmmftezs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jiyqmzsf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tndcyhul.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cvpodnoa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qdxpqztg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3klibvtgq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3occxlvnc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sgucgebu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tvfsxhri.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3beaijenj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cjqknwen.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pvzcaozi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ecelgnkh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lhorkknv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ejkabpfm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jdtecfqo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bxswivlu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dgnpzlxa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gmyqdwva.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hddhhfnw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lalatwoe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yvbjqrkx.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rywqwjgk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3beigifnp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tqdqnpmw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lpgjzryr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dwreyncb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mjzfmare.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jchjljmg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3exutiwxo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ufbxlxab.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3dkkxcvoq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dhypbyml.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qimkqpmt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kimnmegk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gjscgxcj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ukewwfzl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dkdityfw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3eiaainwx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hyvbsxcc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dfamevon.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3etrvfkvz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uuwpotpk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dmnopycx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3fmhitgem.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajqcrrbw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lwxpnnlb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jwzkbmne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3smnsnojn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ptyudhtu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3slkubxya.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3isohotqh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zykvvxsy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ejbiiilx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3tpdhetzj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xbgrepqx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xppblawk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fbftwoae.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sptynchg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3zsesqgao.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbaxdsdv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3volcvfmm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3btimqokq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3flqkaslv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3yhieccwf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vldkrofa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hxnmozfm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ndlewjfo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tbjijmmv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3noydxorw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nedqbnmq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3emwhodoi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ezqbroyq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mbcklwbg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ibpcgtmz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xodexldf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ohgfcodf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qogbllqj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zzzpawrz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3yiqwslmu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3erzzlvzy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zfffgggc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3cmzpxtbs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3frddtvmm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3slsibdnr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ofbmwlij.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gafgffqc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3blxmuzie.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3duoyefuw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3nkqcvagf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ugfansfa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3flrfcpjn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3atujdylu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qeipnqti.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bvooipxy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jsqlhyhc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eodfhzzg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3czpgmehg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vfculzat.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ivpmroyw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ithzinsy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ugketyqv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lrinvhkx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rmdvksqp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cotgemeb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jydhwlvn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mxjudtwl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bstyjass.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pixkvcav.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ribvznlr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3balnlmca.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3eurgdpdw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owbklqan.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3edcbovct.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ksywyqkz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jwexsoct.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bmliikkp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rxexxcfa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fyekklcl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fgoyosuj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wkvmzlby.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ytgvknfc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3skkkxvxf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rjmqydco.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3uanbhvuu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qaovoftd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gdlhjhse.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pwhlelgo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ubupiagk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gqbthrgi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3amylyorx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kikanmyk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3swufsuzv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bjyxulgl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3clxwinky.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qyvzuqzl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3peaqdcoe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rqusltui.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mzolegbw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hkfvxbrn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3helcikdy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mdydgnhj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wlfckhsg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3erwpkdky.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mqrnpbix.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3edcknobx.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3xfofgsyd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nkkncbfw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3malkyvda.html


<!-- 参考信息 -->