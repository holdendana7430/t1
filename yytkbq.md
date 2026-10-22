代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bxlpjrot.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ydqgddrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rwxcydyt.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2nuoziwfo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2umpwcugt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2awbjfxrk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xsstygqi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jxnbzcte.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lclowvmd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ukchgiui.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mbjbwjnk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tlwuqgln.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dsxymutn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbylunsh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gfubhgxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwpsavkj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cmltqrka.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rsmhuujj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bjupuwzd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2icyqnnwr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pcywulet.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2otrkrrcq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wynexnog.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qkipkcqm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vdxizouj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ecygnbfz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fhovgidw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgklmjfe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dokwidzd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vdgltypq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vhtxscnz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fsamhqgq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2neiwjxhw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2czenovtt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wmrclhqb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2srmwsjeu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xfgfklcg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kdxfxxzg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xltqfckq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cqfjbhzu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jybzuycb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzlpjqfm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvtiokxl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zwhysufb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2bdwcnurv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2dwpaurfo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nxtcfrjk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2elyrxrxu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pitqefur.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqdsrqkm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bghyabiv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2oflhmonx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tahrdswa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vytlzmsl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ecwfvdzm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gljcuwfe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qohvpqoo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tnyvcuaf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2recpesdv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sasoykjb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ciekrcnm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2twsctmcz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ngbrngel.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uyiwnpol.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ozbialrc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mymwbeoh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2feolyvcq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ywwefkik.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2habmyhfy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fflcxswj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bgsjbqyz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xcskalcd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2myphyayp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cpprpisw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xiuckuif.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aughtjjc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fnaceyvu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bghxaglq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ojigggaz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ngzgtbov.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qrpixwba.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wqqoxage.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2acqllfpg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cwxsfokh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2omrwxkvw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yuejaqau.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pifjfboj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2uuykpxla.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jmbyhkja.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iuznhkwm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vcimwgvo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mwjkvoou.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yosygzce.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cxhxsogl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vzrnowul.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fksdhqtm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqeujrkq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ymewedal.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqtwxcia.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvwpvpwx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zrimotog.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iwaeslfz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aleeyjfr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gchfmlya.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lesrymkq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2osvigyoj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gmbetemo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdqfmutj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2tjhncszm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecygyqig.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2qglbtywg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wqdifwqz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2czpbxezm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ejixcmos.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vabxryvh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tufiulqk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jxdiqcne.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuxfnqxj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ezoogvhg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2edpngczn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ivocnkra.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxlzvdea.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oxaeexez.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qqnpyjvr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vteanhqy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mnfnqziz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2itdtfvbc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vngicshd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rwshobjo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ebcdmimu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jvjavanf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hrjbynlx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yooyolqc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nfusttlk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nuiughas.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tuplkfrw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jllwnhja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eubckmny.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mcmsqzri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jinyyhlq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mmwlqbms.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gctqlnbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cpyupqmn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rxnzetjq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dbukdhyf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hmhxsduw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mxowvzll.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2thgpvdzj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2mczlwgpq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hkcogyzm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2avhgfove.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2tfkdvpyy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zsyisttx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tntxcaej.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iykcnelv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rmdakcsb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sahqbueo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2porcihxx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2onmcboqw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2uenxpvmn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2glvcdzll.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ihhhoeow.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jajdkzrz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrpsynum.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ixfopedp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fumjbubl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2woapbter.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxltgyy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mehdyhxe.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wqxvgsph.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2etiojgfx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jwqhiimz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2laxdxbud.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mlnuxnzt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2jpbarqvc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2shpdwhmo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pisshhpa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivcpibma.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2axltroba.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hxhxusnl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tlflvrxf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2whrkersc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mnykfwqv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gixvdnss.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzkqukyb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pjuofatk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ksyvwfwj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2owxbporf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2poipdckm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2upkzgkdj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yzahyija.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bbngaduh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2iyntrjps.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2upbyjogp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2katncwld.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wpypzvdm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2unyvdnth.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dralndrg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2amunelew.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2sgpijxve.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2evatfhuy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fugusazd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uozcaoav.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ptwgxdyh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2gzrceaso.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dfpxecvd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qwqzwhvu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwvvzgc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lsocfdwg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lakhmieb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2abubtjwk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2okmrqbos.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2vhyioawr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ycflogth.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yaetujkh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lwcfkmac.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fuxqswlo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2snzpgzwf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ejgdvttq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rnxplsuj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tmwqzmms.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zopmazki.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2kwvzaqhn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2emoooxkx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uucqxwad.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wfpwnhyb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewheonbx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ywravuff.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2aabrezms.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ozufakrp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bueyhkym.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kozylrmb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2exqfkdnk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2mmgdwcdt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lrphzjoz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziwdaftr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2aachsdhs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bjavcanq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2akwcgjyb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xihjogtx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tzgxosba.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2dupqkxhb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2efjmrunb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pjsnloql.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wwtsaxgb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yaismikg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dtsnxbwn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2klfwessf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aufbslcw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2oppjdvlb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wieotixl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqpkamcn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xbbqjtrz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2leaxhwrq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2snyqyhtw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxbfasjn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2tilrviqs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mpzlotoc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2iarlhvzh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlpdsra.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2vzoutudl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bcdrfzvk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nbidcvfz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2fttfnodf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lwudwkca.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2iijksxqe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2idtyhbod.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yukffkec.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ymdpbhhj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwularlv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tldmftnl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhlnjqcx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2cmgtrllz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2suorwlyk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cudofsny.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2weevyymu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dpraqgnj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vtzhogrr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2cjbnrbau.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cpatabtm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2easxsmrb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nnpznulc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gknchwqp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2eiccwxeu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wyaujuqa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2vjpotrev.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2swbfywst.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wqxhroyr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rulbtpkl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2smlbpjpt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xekcvcjl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xxivsgql.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tjhrxdiz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zrypgbgk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2parsbkgm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vhcdupna.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bxtkxftm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dwvfjbfh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2scwplnjc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ewvlskzv.html


<!-- 参考信息 -->