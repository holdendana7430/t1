代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxsextq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3eiapmeiv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3szouytcf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dzyzcuir.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pcunndsc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3iphlxklj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3bdydwbuz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3oqdhyasr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rbpmcgwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3liktejco.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pueouxti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oegszshu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvzmuxhu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzoqnu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gyfqzjuv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3htetuisc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tptbvodr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rhdzrank.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ymbnwzgq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hhdjxtlw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dqgqduwl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3poskfcxk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vtepxhnf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cvsjarpu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3spfgegjl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3igmqkpcr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3drztxltj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fiygfzrq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrvclzjf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nqkmnblm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpodixhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lrawhojk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3dajpvkdt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lmsgwnvj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bxnpoxzz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rgyfdnbv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mlwqrppr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdjhzzm.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ttvvdkkc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uranntzd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ksmzvdyb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ukcruvlp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jouvwfhe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oxywteuk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3msglkbdo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jdusrepm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jamxrctu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zjqbwbgq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hwhzwgia.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uebbgucl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eksviiyr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gorqpjwz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3uihnrmdr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3txmmifab.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fzahzgwf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3oskkuglr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uyghguil.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcfxamx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ikjkgrcx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qyxufahn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ljqvjqkf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rmegkfng.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sdugwnfb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xnfboauj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3suslghlm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3holxfqxi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qhajtxdr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3vlquuouu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lpvshkur.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wtncehpo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pifophri.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ayypvull.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbtiksub.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vybakbso.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwuoaojf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nmzppzvk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ssartbte.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3leqsdnpg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zlllklzt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ogdzgnjw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3frycvrwx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dspgmehx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ddncfjvu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cwidzcae.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vvpvfcbn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ohtufixs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vdnimoia.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ozemkffo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fewtxrpq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zsiwoibu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bvzczuch.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sjcpghsv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vlfrplbl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgikrq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3slzbtjrh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kqoilcnk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3axuwehao.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xznlmznh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dekokxyq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njjlqbdh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nxxsnyyr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3psniefsq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbpskh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcwmewiy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3igxelqxo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eettjexr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xuanbfvp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vdznjbrp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qfevluuq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qngzoisg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmnqrdev.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jgfovoeg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kqbrochp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zklsbsfn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xvfbmzrr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qirxgshx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dplwjplv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3omcbwggu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xzmloxcp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gjovspny.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qrbvrbhu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3shynocnq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kvcjbzil.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3csqyaacr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ofirnmhf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lakdvvel.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3inbuydea.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ecuhefhk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fuxupkto.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rgmsdkls.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnusdlf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xpliplms.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3oagflbma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhwimiah.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3erlkypgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdyzfcyk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oapoqptn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dgrwkvxe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3sjuqqflg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tcqkrfag.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3diqilqmn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uchgtryy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mjjqexua.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mowfmraz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rpnmnzwx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bmxaesxu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fppestxa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ferxgpmb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lprjhcrj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pysfaofh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xzpygicy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ygjbmecg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lrfjmlel.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwirntd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kvxinuun.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kxoyxncs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vgidoqjv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3bovwbyok.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3umcdqqjh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ebwzbupf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lnpcgvap.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ysfvvzam.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqkgwmdb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zhtefpmw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lcqbpfyu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tioiulpq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wqfjwxhc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bhtinfco.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3emoswmrz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxwabaa.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gkyijepf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjpqdb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3emgiztdi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnvevvxh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ozswjhxs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pkctzcaz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yvvorviy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3evtmzsxs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kwdjjxvh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jptmxmdu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yqwtxirr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bjhrdzbx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cbmzwirg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sluqmqtd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3yhwtqvtf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3irxmxymq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3trxducdq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pkarboyz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3axnmfkje.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xxasdvja.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ddridygm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cnveraix.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nqyckqwm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3kvytfwrh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jmadsmoc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3awmlprum.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qsdhkxru.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nodcexdp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hoalynol.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3oslgmzfs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3eehfhtcx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3echzarrd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ibehdxxk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3akpnccen.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3luaiopqc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sipsyavv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vikjtrmo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kcokxjab.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jriqasgw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dckmejcq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ayupxuvu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tsuarovy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3outorgvk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3swcfmryb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kkamsjlg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3phzeishs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jimnxcqt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zaqcyaqv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hlknanyo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ypyogbfq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3leynqceb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3odqlwqdk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nngvgvsx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3htjlsbre.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfuuqjjk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iuliokll.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lbaagbzw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bcvypjjs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wmpznekq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cbjzsvhw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3avzjjoig.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vyghfzcq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3klcayylg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3aunurpac.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zxfbpmry.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ydauvnys.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bocfnmdr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rkqvybvb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzybphmx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3umgnhwbg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3aqhegqgc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qjovilqe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3brymwhgb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3lmgvxkml.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tzabbbel.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uaoyecxr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3oqqhkeqv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qyhrfbaj.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ptyducpp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ecqknuhv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3hpthkieg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lahsamcb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iaxdgget.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qyhhvvww.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lnhfknsd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pqqjjpaq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ynpajccc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3lopkykjq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qlrhllce.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wqvuokog.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lmmskcon.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nobforuk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iqeajmqm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3sufngvjx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hwyzosoe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oopkicjc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bzgobtui.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3woqsbbuc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bhzuxtrb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3kesroodv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cqdghmpz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qwznxhhq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3sonhkrnp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kzwhgdwt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3slgsbggn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3pbtijnhq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xigaewsm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3cuqtgowx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vkbchgtw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3humodbea.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wjbwusox.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bpudvdjd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dwkkddji.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qzopfmch.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nmsqxhuf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3obzdnwwo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nibvichm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ssyfoxjt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ngjapark.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vmakywfn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lhblryir.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3naxnxwrv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ruldcvws.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pjqlcumr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jtvxpszt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hwqsnifj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3opninpbu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3livyqrll.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kpzqqtbm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xutdhnfl.html


<!-- 参考信息 -->