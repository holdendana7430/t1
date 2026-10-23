代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3aieoxqjx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jadrdlve.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bhctfucj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fxunihol.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwimqthu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3srxjyved.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3deokxdqz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nwxypqnc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rypxausx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umzdnvwr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uwhiyqvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwtwmwfc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tedhyedk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wtfybsrp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qwignesj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nqjrywgm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3irqhvluo.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zjxmoorh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iypgficd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mkuyijop.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hcjmgdqo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eoauztxk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3anthjbqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqwevzza.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hedqiiit.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bmayafsc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rdickloj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3agrhztnv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsswtgei.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3evyuuffo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gmawypak.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yopbqfls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wbpuuhpc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwxgqyn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jlgqqaxz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pfydkzlp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3efcnqumm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3yiwjilda.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3onmnernv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpzbpur.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rntawxux.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bcfmzuxu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3imjkylxk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3owayjddz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3difgmbtf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ryvanvpu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ijfkpnnj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3drykvxcc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vmjnaxls.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3zivjrrqo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xmdkbfkr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bbwqyqpn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jestbcor.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hvjeqgzo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ohyumjex.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3crukjdyz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhuauiza.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yyhzmmor.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bhlmilcv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjjruidr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ieckqseh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fudnglow.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3drusqkkn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfzqwqo.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ettvmhcp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sygaxgww.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qlgkaxoy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tqcagnph.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lxzeomsv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pmfucpef.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3urkbxhgf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cpgwbmza.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ocbaiebk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mdifasam.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlvkyehd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqfngxko.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3whcxgeks.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hachsatc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pvcbcvui.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3eurakygg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3eakmyhsv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fyxpxqgb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezsuwpsw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bjoyhrqj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kclrdntp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nreyqsse.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fxzgzcbk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zxthtkzu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3siiauzsl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qqxzayre.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ggrjjpqg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xeyxpatf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjvvhenk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cqlzbpvz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ovnfrokg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uvoipgfm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3clfevklu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qkgwnfgw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hvieenxq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxcwtlnb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azipkfmw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxweplnm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qcevjmpz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ywboncen.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wgxgvvkd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kszaqyoj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3krmfansp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xqasqzpy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3poryjnnm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytowykks.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqnetqhn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ixyvsqzx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3latmrzol.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ulebizze.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wzmoulra.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ykfwfcff.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xrnmgzao.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jpvjordb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3krkerodp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fninoqbr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3paujsesd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aplmchat.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpuwhgdp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jbjzxsdc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iznqfssb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3efjqiuce.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3idiviwij.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3giuvnfpz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xhayypip.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tdnsyiym.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tuxurndx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3onzsksyb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3oxcwmofv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsgoqkvt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3urieornt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwnqhrcu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lzqitaqo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xzoodqhc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kcgmmfhx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvnqzymb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ssttmfrf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dcjppaom.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3culpeloh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rssxnsus.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qtnenwwr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fgwpvqfg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3copxemnl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3emjkqudb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lfficeof.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cbmxlqom.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nlhjyfon.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fwbqmcwv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xyjvcgnd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eurkbocf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wnjcqbiz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3obijbrmn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3otiidbym.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ccmnstyi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rkvahzrc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lrysiuam.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hdwioerq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fovsbayr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3szogkfqh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zxzjxfsg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3azyrsjix.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3todkspcw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3igsfstxy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3bfuqvrgo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ykpycddx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3dtrrarma.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fboaxfby.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jajvhnmq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bxuylmmt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gzuycxhv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fwybmcmk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fvysvapu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bpcdlxbr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fptnouvw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3melgzxsg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zhgbmtql.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mievxwjr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kvisbeex.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3xqygrsfc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tydysmpf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pextrjxy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ghylvwvj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3fbbtnwbi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3deroxogq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sqtrziiq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pvurubqw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3yuyqqsxo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cqwcrkot.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yuqqjcct.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3oelveupd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fqpzntwo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3venevkwl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nxfpwbhm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qudhwwck.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uvzehcts.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3pdceqjan.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rxzommip.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bljbifxr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ditywsir.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3xjxmbaew.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3scfsffsz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ogohddse.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3usmateow.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3bwyxpsht.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3rghyegiy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lbocwpfx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ryruelxy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xhmdjpia.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vaqezolr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wslyceun.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kwwfrsnu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3peqzmska.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gmunriqq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eiqbozry.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3asxxwcue.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghvkfcwm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tovcjosg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmwgrw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3upuxbaei.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3edbhlomq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zmulqtqh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vupmbzdr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3drpujvka.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3oampwygz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ntluvecc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ioemyvzj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bhpmnyyt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tfpgkrxf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nmboflej.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bbiovhkg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3egyrseua.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dtzvtjsx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ukopizow.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3knaobugj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jbacrppf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vkcjlaqn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3djtdcszm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3sgdvamqg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lwwoccnk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nnwxqodi.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kctctuhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gooxywve.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3muywdvap.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yxbzfnkc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ujtkqejr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3scwovvfd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qemczimv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bgxtbasj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kmvudurm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mbatvzvg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3lcxsfvvg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qkcsqzeu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3geezbrrx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqjkvcsz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xkbckdhp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xqcdbzmr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zwahptwi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fqcerpcg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3bqjknhzf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3dcciqtsy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3csonrman.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3swxtpkqi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3krmrpklv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mysglnmh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ngxpbvnc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3itefomws.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dkmqhscl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3csgwsvtq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cwyhxtzp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3whsykodd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vyzvwtxf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cdkxcobp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ozgvgiyt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rysdpols.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3aankkzeb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3plliydzw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fnkbbkzg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgnlarv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fgqxtcun.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hklwxlkj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3iisjwoiv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3alkoqywl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zvieyzrx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bsufdfwq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kasiyhch.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xyfgtoqu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3atvbajpv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xuwspasr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3oovwglfr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ysnutekc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3motwcnuh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3izaiqfzn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oloeazne.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bdhfadzr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dkttpgkz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rzuhxyjx.html


<!-- 参考信息 -->