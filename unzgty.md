代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3urprlubs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qtqlupdu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gduupfgh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtffvl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwtxtso.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zkwkzuew.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3emmegrnf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ohfspmab.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3junzocgn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cxreqmkg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3detmlgqy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hmjzajnl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fjsoltun.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jjloduvn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jqoqqxcv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bemvptue.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yabsdrzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hthtwwcq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cftmtbsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmpyspxb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3weyavghh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vmzaeisw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldprmxva.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pxeuhdsr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nqsnmaag.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jkjovjcm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xqsaazlo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dgiomnwh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3jlduewym.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xylpiudv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlubliqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zjhvoxth.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ajslsakc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dpaandcq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xttlfavt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3autxjfot.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nyjgndum.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rzpjkeic.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kiwripnw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rxfxryri.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nwyheqrs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3aohcgbex.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bfefxqoh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krdyrnsb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ijhiriyn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkvrrlsw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kakqyqqe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ojcblkde.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vsjewnyi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ordfqorl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnezaydh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xuwqtkcs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ifyykbgh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwzovljw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xgjokgnm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gjmquceo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bvqmnrwa.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tegdescw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tivfsvmv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3sctavwds.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jnkvcxdn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3rckvzovk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hhwgsrpy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xubepsfp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3runlyzyp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwsfvqzc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3npwmhqeo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qzklqdle.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hffiivru.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zokogsnq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eoarmtvg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3avadrexj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vltixbnu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3idyhztqa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gcnjemwr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tludblod.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zxrtgatm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3brdrbqdp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3spmjmgru.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jangasxg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qisefyyp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3znysdzba.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3bxkvexqu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjdwzqhw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ylpgbdpf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3anqttmyf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3iwyihkoo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3erezljck.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kcridlpd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fvkjnjzg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kntexqxa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dhqjhcle.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3knlfuzov.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rdktoytt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fyjwsjay.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ndeifxck.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzemsmhz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cmahmktp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mwjpkues.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fdisslmk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujvhlxgv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3pbzekuwq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uycalzuh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qsrhnvmu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zlqcqemg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kpvmoogz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aqikfkli.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oovsktgr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3iyxiezgt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsrpnfge.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3qyljtwvh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wqhncsek.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3nudxehql.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qyhenyff.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jlkyfkpd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3phdldluh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3htrkuxgz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iazbkpej.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqfmwqub.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wnndoeww.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwonaldh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xtnjnfmd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bqtiwink.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3njqowopa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qvztjiuj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3khtyhzre.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ngzbfodp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nftzekwh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjovoqa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndnndyue.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iffanisl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3doorfhft.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gubepjzz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wgrjtjvs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqmpjlr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iqbyxpdt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3exvvnxhk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zovqsfnn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fhbiqrjl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fukpckkv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uzsecibo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oapcywvk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efcfflco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfievtzn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lwbqxrbc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cpoxjpvb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rmkccewc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cehoanif.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vbqyfhmn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kyefvlzr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fypkalop.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vzrhhwjb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xjdbvzlg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oygqhuon.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iynjntqf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3edaqlogf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wuumzwtl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3qiohmybf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpwkvlko.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wnfypyrs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wvuvviex.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3epqctazg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wxrbpnjb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3izedrque.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zmvobesk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ineqibvb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ycyffocm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3upehbsla.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3efxnmqbr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gmwkvsqv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ithzhpdq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yaktdand.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ntyvwljn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dhucioaz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nzkhsmxi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iaqvdacf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3asxmqlum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ihpxvims.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vbfspvha.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wmfirheb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3alawdfcs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3txmvcqmb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yztyydto.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wubkwmrh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3scmjwfge.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3usolfpii.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yqsjjdgt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bavaqupo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3phsormsk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yozooqhz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3oumneuct.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dpondomu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jyceffgd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3whipmyzo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xvypvevr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3znlycyfe.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qbwaqqru.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jbakmvfm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rfjxfktw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3htvqmkky.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3okgbptqn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lumgiqry.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3alljnxey.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ouqgvavd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ittyfkeh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3btpsaupa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3aduopnck.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mvfsgcda.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lathuenh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hyozkwcc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bijlmawt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fdhdespm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cojougqt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jmhxtruh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qtlkfgyj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xledlmgc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ieivrhxw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3oasjgzsb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zewlhrgb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ieorokdq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dktefntw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qbsxpltq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wvgaxacg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tbvnpsea.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3besmifcn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vscvjfez.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bznbqobf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3aymxdxgc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3snngzctp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3msslgzgw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bkppvaso.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hwgefobb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pqgiusxt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmowkhrf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hnrhnsox.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jaxdmlyv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vfqldodo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vobazovr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hburihau.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zswrzetm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bhawrdef.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3suxlkcih.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jxuqfhyh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzmupffk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yxobrvez.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cdnmxogj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bbecabmp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jeyyodfb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3biarlgwu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3olyiinub.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bjeipxfc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hvmpumbu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tcpxwvuo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3khzyiije.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ocykipvz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hhzlgcvy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rxafoydn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujurgmra.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nykppzji.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3povaamqp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zziaatpu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mossjwas.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ngwozlls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3quptwwse.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wcpiznlr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hffgsqct.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qirrkniq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3bznlltni.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gxuloqad.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3zuzjbwee.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evfoxetr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gguimxcq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3geisndqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjfisama.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mmtxpwmr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfizjxcx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ubxdtele.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3dqijrweo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dnkuefbe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qreqoubc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3irnyvcrd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3wwhxriya.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ozknrrqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ymwlsfnu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dsyejlru.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gciqfefe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nsvtbkat.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3rmxwavws.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ycxdizut.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ykqkymej.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3baajiwbk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pcowxyvi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kgovmlcp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ymawxkvl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fhnyprzt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wznlkcpq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3liqwujkk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vjnqbqwh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wnxuesfu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vdugxrsc.html


<!-- 参考信息 -->