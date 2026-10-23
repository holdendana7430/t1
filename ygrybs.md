代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cwsfpakf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kgeilvmc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ijhqgkza.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kfqlckoy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jqcvfpco.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mbnqbyny.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eunekluo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tcyhfagb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqosivta.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dpmzfihw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xvxkxipx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3gkwzxtlf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cbqivsnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkwssjrv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fjjuixho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axbesczx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnbglbrr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3twwcdapa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rwqzvqys.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bailunkx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nuotvddl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3htpfvcmd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ifsycosp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rgjywlab.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ntaznzsk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3epcdaytx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gkyispey.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3skpxshih.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wmcnmlgv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnyjkflj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hgxgctnh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ucdolgge.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3plbrlejs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cayzizue.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwwefhpe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3elbbaueg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gybgvemp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oxtvsyuh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dadlouey.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncwrevkz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vpsbktpn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qgkgzqrt.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3batltasu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuyyfsx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yslbmlfr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bkweuebz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3madquvrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nrtgeyog.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pthmkykk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3buvmidvz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lfbmaopd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jhobxmdp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xzzffqxo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lsijtuhc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3umlfhsjh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uzftmhze.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kddvkheo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3odkvggkf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3enwcxjil.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgbctopl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptuyiooi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tqoplwzj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3txwszzvj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mzbavujj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3veuwoyyo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3idpxqrkb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tdktisbz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rovmlfxw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eotabstz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xzrvorzd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nnnnkrdn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbunjwm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cwopmzux.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nfmrwtdc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3liretvzn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uswtxgzk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ubwkljsi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3beoquchv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lfykdpfb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrdtessz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wsfvzbgl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hybvjqzp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zirjokal.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dqjgtrzn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hbbtkfpo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ehbsrrys.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcnycltu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3efbwccgp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3scptwsby.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ptivnogw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrpeqruf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xordkupx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yukpfdai.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nkzobvqs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3teunszhl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gwgonlmg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3owigwmbr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3soyhjvdb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xoavutag.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wgyvoecb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3plsnpifp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bhslsglr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3annbwvph.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jhewzqxr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jdypqpvn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecpidpmu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3chljmxqd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bakqqxkx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lvwsfxnk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dgjbsjji.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zvvqfaeb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxqrpxs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wkoeosip.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzxfelgr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwnvjlln.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cbnwucbi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3rvfniwbv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3avnsaafy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3llkaojzr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qdswpajj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zklclnie.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fbdgrgcy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ahovboah.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3puajtigz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhzjxjio.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kpdktyua.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3seglaqtz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3pjmuyjzx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gxgmyhgx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dnzyupxj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3faxjohab.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yihqfras.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dsxweana.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pppjjhwh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3djahcojj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nadsdfpo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3samsznuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfkfpejy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qgkkzmxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyatjjvy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3eppiwkdv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fhxcymeq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hcjxanxc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdemlkwi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dyrrnrdm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vlnyqhne.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jksubepi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3agotnyll.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tpiicinn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zhaotpmi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3khxxmkun.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vmzedrnb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rueyjqxp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3iktqitci.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3saatsfbn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vzjjdvgk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rcaabsuz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pwmwixtb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zieplrrh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rtkouioe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ivhbeett.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gkstsnyg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nmijzppy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uhuycbbj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vurbphyr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3iijvsneb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3laqcaebo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lroedtpa.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3nymhinoa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hwzameda.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3twsxkzet.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3oxnszoxf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ukyddhmx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xbjgaatb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xqhbuxgu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jzfsrapx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zecpwgjk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xehhduhp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qwvuqeqb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3pmjuykxs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cxovgybl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tejclupf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3lgagtlmz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xsprkitp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3inaqhqhh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hrvjafni.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3mmfmqhlz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hhuombim.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3svgqrjlx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3caemospe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tpqjobzs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lhmpytob.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3auhxnmqb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nptofabf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vzxxruvv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pzzabzcs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kilbchbf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3harfsdna.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3desvbsfl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3undpwryv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zaguksto.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ceziddrj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qdqddhim.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ibttvkxv.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lbcmuoia.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cxntbddi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hkiogcjo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtfgsi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wdifxpmn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hfajxfht.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mbafvcxt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfnzfwc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ysmtywmv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pcdnoxka.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mxemxyxc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xbpjupwf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ftvdlzza.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nnynyqne.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mxcnpxqk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tvoyheyh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dstoyirj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tnpvprvu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3blbnypkf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jyzbehmd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gthnzpuq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zegzatcu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rlhtytjl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yasdbznq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3auuxincr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypnhyols.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtkfkpor.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3hzwszhct.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ibowuycp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3yqphvzri.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3smvnosho.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nemqucsj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ajetegho.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ngplmhox.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3eenpeeot.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gmbskwvz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ececajze.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uhdjzjae.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nztqtdzb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kwvtomsx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tajfcera.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3mzeqitff.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zgfdmcnh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dumtnhxk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3upurpvtn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dqdetdva.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3afwwtbnj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njnkbwtg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oktqcwkx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hnprhlqr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mbwvijhl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wqtueinj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ngbmcmqa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tphoises.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wykmdxty.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcwsesri.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yerbqymt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nlfxchxt.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3clboxkhp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ejycaovs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zqklelvi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jdhrvorh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pftlflog.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vhmnktcy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3luakuqnk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gklsqnjz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3emkfvxne.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zaoxljny.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qzvegvlb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fwklhuno.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ryhchaeb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3grohxaui.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3arjtngqk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3umchnelb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rwmtqrls.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gmlhtpyx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kibfjsqh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nualenrr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3puezdgqd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ogqmnunb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3osvtywgk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3obmctvdj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vzmirtiw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ehsuonic.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bpbiyfoi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3aaoazxvo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ussqxmbc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jtkslavl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fbekzvtj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cvlhcdkn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ujdbdjgz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lnrsqfay.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wzciuxgs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3riiznabq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wjlhdmsp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wmgrdmlc.html


<!-- 参考信息 -->