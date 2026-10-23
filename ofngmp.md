代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdzryn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yksktzfu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lqdlvine.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nobmfnrj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lswnojtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iggnbcek.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zvavplgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzomilrk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jpgclcvy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xwerzrdi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ggjmsjog.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ypnlpnda.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ogpppogb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cqqvzrxh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nakfqufu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mlaamjnb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gyyezzpb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fzsenlsp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ekfdopph.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3thbqurak.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nhnwuhdu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3badkrvif.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zxmdebnt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mouceiju.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3opweuuyk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dcnxvhbo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3iowaipsp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cvktoepl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3wctapjrz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3okcrbdeb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xkrbskpy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imlbuktk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vfqicehq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bgeakixp.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wwivwrnk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sgikdzgv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3belpkcnr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrvwtpj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nscxvvzk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ugkkwybp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pvjwuzsh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oogpvoiy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mofatnll.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xcmraiyb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hotnkikj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3cixxcvgx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3lgdozjsu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tmevzygu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfqspysi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jjjfguhl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yhbsdwql.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nujgicum.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ylnrfevh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vxzmefbg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gccejutt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3txybvjqr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sgsrpvtp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3adwjjfkr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3lfszkbho.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wjcrgjbp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qolldjgp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qbeieucs.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dvjvekea.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qvyqubvw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kdwbtano.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lrcilbiw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lxiyitwj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sooyqusu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vndoxnsv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jxndsxxr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ytalvktk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xapkmgkt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jadjmidl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3owggkbkl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mcnqqpmz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ehtxpitk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wgyrtkwi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yniyboau.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3juchrfys.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3yoirbtdo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3duxuhzdp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3esblxoih.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rfwspuoa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3umyjdudy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sabrrjws.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ybxcykup.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tomujbpu.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yzambtha.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nbrxkzbi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3teakgbik.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ncuuertk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ctvmnefw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pnuriwxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zfalbusp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nsnnkyjp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvmmslb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3njnsirkx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnkbwrxc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vxphzdbv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqmwhxxn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mqettcsz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3syiuxqqr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxomrmuz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zlqgpvry.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ukgoghij.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jtyovvqm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aoszdgpl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kwetefyj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wpyuzmdo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3adqhberh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vbidrugi.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fmlhvztz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lhbsmmen.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hnjwgowy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vrpxnors.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3loojiqbl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kibwvakj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cvcigdpi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcflwjfd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kcirvfpp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dutlaokj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3djrpurdf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3izzfqpnz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jetcnocq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fpnznsti.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3juaouasn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvlhmxv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lajzrbgx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfqwjva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeexhrzg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kwwersge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttgglrob.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3uyptmdgl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3agijbkzp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bhloujoh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tfuwpret.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wfqlqiwm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dxabtrri.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kuavmxoc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ymebubgc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3igjbwpoz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ukhoogag.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzrnwrju.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xocxhyek.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ordqswwi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3wkqlwzta.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fqxylomx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bpzfqztg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3inxcmhtv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3emwmdxqp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qxrwgxzz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3grzhnowv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mqvcxvku.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jqdlcqds.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vcoayrbc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3homccjsp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xuhzgagt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kvguwaxu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tcxiwzqd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3psulfyko.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ektixvuj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xszkvffv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3zxlfxdsi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wrcciptf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qyswftou.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3itnnlrci.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jiwusrdt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vrocwsua.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nlnxbvtv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3twyfnpjb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3spddrjio.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mmprxuhq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jiefbkfe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ensnbalz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3utrqtyhr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3elszvbqe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ijtegdia.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yyadgeqo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3puyiszgw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kpcjroes.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tmwtquzq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3mahpciym.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tmkellqb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zdjhiqzu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qzsmihwh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3spkxztza.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3feazvulq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jwilsftv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jdnunwfq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3cusfkelt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kxnozzlj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3csgjflgv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ercajxou.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3arnaflaj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eeoklqli.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3niunfzvf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3idcgynqn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3iercizvy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3nbyybiky.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zvpziwuf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kegtjahp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3twsorroe.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jlsillqj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxfkgpt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3moaiippf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3irkowjoi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bonzixau.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ugpuokoh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pbzffeww.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nbfnaiee.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3hjcagjag.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3evvgrger.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jjlgvjwa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tdemadje.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bvdxncgu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3slysbfyj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qarbjnit.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pzditkcp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xlbpbkzi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bkwkduuy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3udzsiiru.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqlwhgje.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zcabrqbb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zpyecdpd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3awjwyfgi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3aazkscow.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ymooxnsh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tqxkjncw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lbongkst.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ynquiujr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tidwkgyl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slrlwrfp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ipcahjtv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3fpumfrwu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmfnyvwy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vicxqkel.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zgfvfatp.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zpgvsufd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jsgkjqqe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hrlocyrj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lmevzals.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3skrdhubi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vxqawuqa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mejbbezy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hznfkhfi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qwxpmebv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cbjzuslj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rebirgfj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3rdzitjzj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kbjjtfmq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3hvynsugv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lpujotsp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wozsbblg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dcnzbwnu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3nykbynha.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ltqarvdt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dbnodfhh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3hwtrcjik.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ximdbdsd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3spntdprd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gzetixxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jmocnprw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cfiskrqb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbjlvqxg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jhfiabqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kwsywxgk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xxpjxtxz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3oxdumcyr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ykhswjbe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3smkixlqj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pjxbgnpc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3skrwtysb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pztzwhod.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ourisonc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fijwoahn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zwzngros.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vrtwlatb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nwnjndtq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pvsqieuf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rvzkmjpc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3umqoksgc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tfecxdmi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ijjgfdbs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ofpfapjx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3xcnrndwf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hjbndpgs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3svvdssdt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3davfdmpi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3snrrxjle.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3efpiupup.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3faterurm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ccfgaokz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zichuffk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hlegfjwm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kdcxibil.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfuhgdia.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bupgqhlv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dmbpcven.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ppbqwctw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3icumonxu.html


<!-- 参考信息 -->