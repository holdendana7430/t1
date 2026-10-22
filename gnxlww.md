代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dmourdrv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oioimues.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nwhjklfa.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fpmlgkor.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iagjgjpd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sougcjzv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fivhvqbp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hiphmqzd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrriwmaw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ooeycmoi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ycewvxdb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2cmeqzzgm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vwfwjaku.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lswoulwp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pktbnsfj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gpgvkzjr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hnbnjvbf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jxhzitua.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rmyqfhio.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vaxhlcvd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhptithd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qgcvbukc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qhfaznfg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bqlyapnt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qhfmntbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxvniaxs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gkhaijka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jetljwtr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jyjwclhi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xgkqqchm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qpkwsoss.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2piepimxl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eyxpismg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pfsorhjw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rxwtbsdu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hzmrlibm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lmtkaaqe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ogxoztiu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2idfrqucb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxgfkgov.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hpboccww.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxzugsh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hkzuklyt.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2aaofqvok.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2iqrtynma.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uccbzoak.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jtjadsuo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jwduidbz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ssygmwfq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vzimbuuf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2sdjwhldx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqzlbqqu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2orsyjwag.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gtxcguxy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ycljbfbd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2npupmjfy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kvonwiwv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xmyabqsy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fntzxfwy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fpxohepk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gdzacubm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2orpbppbu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gmcqccdo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2qqzsexzk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xnyhlxce.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2smnjqrzv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mjvkbsnm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rfiilhvg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2egwpqomn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rbmcnzvs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nubcasjs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2eijwxbco.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ugyqbqvz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvqwlwz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2odgddgoj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nwfghxcd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2fqtmryjt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jpkwypgu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2khytyejf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ortnyljk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qpzbbbrl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2lekkjhye.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cmaoibqn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2btqsslkm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cgbmwsuz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dhowiguc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wfrxcegf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qdirhlss.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iuxzruyo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ylhivtmi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2earkanzb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqrfniag.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qjbpesyz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mxlkshzy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tioihnrl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dxoywzle.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bnpjatlp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rqcxnlte.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qxmdkpxw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jokgmnil.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mnpfcmjz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ippbngzh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xxncjzgy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2utvndmej.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jvkeyigq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oebxtrfy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2elptntvb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nupwbyef.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qdpsyhgf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ivdhngro.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vippmpij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwlaxbg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2neaxgzpx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ndjncyoq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2toukuxvm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avbjbdgg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ptbyyftg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2alhlvrzr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wsoqmxbs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rgwucaah.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gyywfyui.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fkszzknz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxnqzqrt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dfqxxnbv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhnvetpm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oybwhnpj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wfodefnp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2iuqpnaru.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yogfakas.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kkwtxuzb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ssvxmauz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrhpkhos.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2syzzzqln.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bccvvakb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xjcwzjsr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hgegvhwl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rwtyuodw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mvzrckjq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rrgfxsas.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yckddvxw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dkalzwwb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qduecgyh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gulejyer.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2nmlarlmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vifilmao.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mnofxzzl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpoudyr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bezocgct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xdmablrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcylpywy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xvepskyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clvemoij.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ljuftwhb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2nruyxrci.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wbdxysts.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2snnbbhxm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fvwecevk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2jxtsncsa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrvxye.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2knpnkzua.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2clybznbi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zpuotchz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2stkyfwou.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2aerywvgw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kjatnplv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bgmpfvac.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jcswurkw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fisdfvbu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qopfmolf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rfhniciv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lwdxsaig.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2aazrizhy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xbadjwap.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2znagpwql.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yoxtfqgx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsibnoe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2npmuropb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kwmgxzpo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxdfcwth.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ypudzcsg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2crsqptbg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xcczfklb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kmyslkto.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wqbgvokk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2psqoeogx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2eokgswrc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tgwjrvea.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2klfovftf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vnhmeuxn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2byxjwlzu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2khkquxqd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2iwsvrfvp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2sbjabqxb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kqnwwifa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2uelxnlts.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2chpiaqcp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dnoxjxtn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2lysrydsq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sxaketib.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gwkwznyt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2pxrnbntt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2owsgdepj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2psfdmyuh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2btxheyxx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fkyehans.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ghlibvmw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2egvxavqa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jdmbrwwy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mpktdowb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gzfsypxg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ryugbqof.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2arbluuci.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bxiqxjqz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xptquhlf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hjmsuibc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vrmsqnrl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2cbzaayxu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2crevuswu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uturoswv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bjfndhqp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bsjqtkbw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2axtmrnew.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjiwze.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wwillxbb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cqnqekxw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rrtuwhlb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kribiyai.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xkzdhypp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qsibpzem.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2eumjgjez.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ktusjguu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqvxldx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fxxebgie.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ubrgzxsx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uurafzjp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2thqqffln.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cbeqkluk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2heqmboav.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xmrsiqpw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbhifq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwkylmay.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2szfczfow.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2cntooaks.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pdofjzmz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aspcyivc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fpvjvrmt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2bcpdqbzw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hfhkyejm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bpexrgcr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fbxgesho.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2opwxonom.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwvrzpjw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lclyqwao.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mergirjp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cedoywqm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ozuxgcaz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ahlruzvz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2sqngucnj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2eertmdcj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wayzggfx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2andckskn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wxetphna.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbqzpgwh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsrhoab.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ypyblofw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sqqwwjfx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gdmxhbda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zravztpc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jsyzzaty.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ktritmpc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zuygpmql.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pfcxbkym.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ovassexq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lbjommss.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oicqgldw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2payihzaq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cfsssgsj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2oirltvmy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yamreizb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2spkjyfie.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2rcenhagi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jozwmcfa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nhkcbnwd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lhlxxogn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2rtrecxlg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ngxeotou.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xmtpxcln.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tstvmtfk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2khsufyjv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zwgdkdng.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rsxnvbcd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hadhbbsf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ifmnwbsv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vsfiyhyp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2odbprawj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2okvzuwwh.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ctzfgehf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gahreeon.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wixaqhzq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ejjdnmnl.html


<!-- 参考信息 -->