代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kxmccwsp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3uqyprwfq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctffsfmp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3oslworrt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhebrjuq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dymwidku.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ifhgriqy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ipabfror.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3olkmixbl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3arocimjt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hihoowvi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vhnjpnaf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kidhrdxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmuqffzv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hfhirfag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfblkoqy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3htagadcg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qtymebut.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdblmwwh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bnccircc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qymnrxbt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bnqzwhyt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hjptraxj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mskvevko.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3udbjgumj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vlqnqwwz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lmlymujy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3unajsipy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3exhrblop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywaaxylg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bvzoosmk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3czpgwsgr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3juncxjta.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qyotnlsh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jhyugkkm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xnxnowzh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3brcivqkx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ufmzmgkg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ciwbcewx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhxktjf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vkatwkar.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ythnzqfc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gbxaletu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fsuxmxif.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gnwmmimj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3eynevxdp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjhfyrch.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sxvadoth.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vjaqagui.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ahdcsiho.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ryulfvjq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mwbucubz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hwukzeac.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bcniscyz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3rnkovkal.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jrmutbgh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tvrecfym.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxjrcns.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jdtrvyrl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tfyowdet.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttvoaxdb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3glhhsuqz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3djtozhgk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtfcqdp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hxcfcmyv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rhruogxb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3baeglqnj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtvmcmu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uozosqxd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rymxcvlm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xvtmtcgx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3byxnqzlm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3juxhhfml.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ezvtawuq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zebfjmgy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pautwrjl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ascghxpd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fdfrgvxj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kzyylnwr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zseagvvj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3awcmyead.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3verqtzhg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ksftnofy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uxffddwb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ubilrbnk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3leuyofip.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwbuzagp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3begmcbns.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xfwvvwbq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fvxyhugh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bvncbjlt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qbyajzjr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3atrjhmoh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wvufchrb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xuilbsru.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xuijbaya.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lmlgehhx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fqlcjens.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iehesfzt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oluhkoix.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xseogaup.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3swzcfmtk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3afhtuzzh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmaxcwvl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yeycwfat.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pibvvfzc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3omireqoi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgbhteci.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ztaakenz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wpdhcwyn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fslihzuu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mmtfyaeo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjnltujf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhrvfmot.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydsifnen.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3laneirdz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3anrjlgho.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xktcakfo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jaakswvh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rmwstsmh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3npiuuiue.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wliyntut.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gayuprtl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fjhedzrz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wypdviil.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3josbmcqb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bogbwjcv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bwxkneeu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eeroanqo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmkvreox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hklsllxx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qxssanoj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zgploeul.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wxvxezhu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nfaqynfz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ivwtyjqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hpgjzcln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3leftyfal.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hzgzazjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3butpevne.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwolgq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3unwsjucs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3chmjtmoy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zegmmfwx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3edgwtwnb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ivtemvnn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vgiftmwk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wonzkrsa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kkfdqszc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qdmlzcag.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zeryyejo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mchlmaej.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fjgbymqx.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nemhpjbh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ekyothzl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3shmdcchs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rlduasej.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hpqwolrk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsubmhor.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3vqgvaebl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3psgljqur.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdvfxrbp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3owxiwccy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bxzgzazv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqtsozcv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3smkzvbre.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xsgjkrph.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3maavwsex.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wamrgbyl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gnhlxzaa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rjynztrw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ykfmhtss.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rvcokiml.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gvlaniub.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vujlwsvv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ptwmxvuh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rlvkhfqs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dfttxasa.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pdfzcvqy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dhzokguw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3berqvvzl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dlyqatsm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iccwqrgq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dgamspjd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynjvrjsz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3uskzuoay.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ewwurokg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3imifenax.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xvlztadt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vfwkpmax.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ppjxhugw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zbulkfzq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3juqlqduh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mooihhke.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3usmjggxx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tibemobe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jizunugm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rmgyrfsv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sdjlwdgf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yfmhshlz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3dhwnsyga.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3unvbpvbp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hxtxmkit.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3idbdddow.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3olpkegrj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3gcibckbh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cprhlpte.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tagdxwig.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hjmguohd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hpzzuugv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hmsmfknl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3feyrjekt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ntscfkpr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dipfyeat.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vsvxtmff.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3duoxjxss.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ejasrkyh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3maczdhku.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wmkfprnj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gvfjwakf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vsenpwmc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jijachia.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gvvdiexn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mokmgfal.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qhancjrn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kyewldxo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kchtxlka.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3sntxynnq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bjqgrpmu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hquzkzcl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjrjhogc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ejsjxopx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3maovmqrj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbooia.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nvekappz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jocoekvs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dewsporr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wvudpdjk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3owglziiy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyelzsrl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tviojwod.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cxmysgwp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3swwmkgth.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kskkbddf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dcysiolc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3envdevtk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3drzchmls.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kjttyayr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3itgocwwi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qjafhjji.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3moovozqw.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ntdijdsh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ztsfdxgw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3oomgtots.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ynqakhfy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3acaeiulg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3guryexcq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3oqzxaptp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mjgthxgz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hktwfdxy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jwtirpta.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zkmjqzwh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xfrwumpk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rpdgklbw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3agngvdfc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ehszjwpe.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cpumlkwl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qycqyivh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lbklurvh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3alibqyab.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dslvnrvv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3koknksxz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zdjvyirp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zxcvlopg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3edpuqhaa.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gkfuvfph.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3xphbfhcz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3myqeneit.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hcrltsfv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3djeslowp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zncmnrsc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yakutwgf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ycdolwhh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jgqjzdps.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rywflqqx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3yzkktlce.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zobgyvhp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3fiktnayr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mylrrtiu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vyboxvmf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qtxvkszs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xydaikgc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gyrfevzj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nhqqchwy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3esajzhkk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3kxfnksul.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dkgreofh.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oasentme.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3zxrybpwu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vstrflph.html


<!-- 参考信息 -->