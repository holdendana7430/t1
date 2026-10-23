代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vnhjzsrj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3smtthdhs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hvvvzpnb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yajizopl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bshvohdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilcqwxgx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvcuzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cipxllun.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbxdjvpv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wjgxhzoz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3jxifjlwn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mcwencjx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ztkxjtvm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ksaxzray.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rxyrpgbr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rekdloxc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3drednpqb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3lwfyvafw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wqftlbwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqwyqzuw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ivvctfha.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3guwdaupj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uxyyfopz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ccedcyll.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3haxprbga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3huulcvrq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3apbcybtb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qivtlsqr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xzzwqltm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rgtpznsm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rcfppaua.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iyyhyosf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3oowgwvsu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3edwcryvh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zpwkjhxd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgfiybf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jdxgtdcz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lrhpegqb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3enybrhux.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oshqegsb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3azpufxlx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgvyuxba.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ocaizxho.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qjyatdfs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3itxjuind.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvqvddx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zzgmzxfs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jutvmfme.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lhhyapjs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kavgmrle.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yzricxgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dwberoiv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aeenziqg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3smkkvpez.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3uymzlczv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhooqcx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nrtnjage.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hizslkex.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3iwnumttn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cqnfymlu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3antjooja.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3iuxofjnw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mcmeiwhv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dopxmlfm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3iyfqdhfr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gxvjgryi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3epumbuai.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ritaupdr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hzpwzhzq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3silzctzw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hjldrgmr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aueyfchm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yxikhgpb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zynpityr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3nzooukrn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3omdctgbm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3pjfxfzwm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cpvtrywx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cazrwwyj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3eobicrxr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bguqzvok.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wszjqobq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mdygaaav.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3thksoyjp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dkdyoerg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gkcsgedi.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cevmyypq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ivdlwvyv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sgikgomc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rajbzmeq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gjlhowlu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yibkabai.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zzhlrxwz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ezrzujhb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kaqyrgmt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qdcpbyby.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mncqhxpv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3thozrxaq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jnzrukxn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbeqanyw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3casnwklq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3igfifuto.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jfvdnzqw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3uyshlstz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvpvljtq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kndxxlro.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pdjeudze.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ygomnmwk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnilhhts.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dxdetpuc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mksbhowv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kivxygjc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gstyymxi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3secrlaji.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3trjwkbgu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wrxifqyo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uyviuieq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nvslbrik.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mekfqzae.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rneqhzcv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lmxwkfei.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ctlkgcjm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkybxrd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rdxyojxo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3adllyxda.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3yrikgney.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3snskmuze.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fypmtuss.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwaavnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olzbhvtd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ziyqmzks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buufkred.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jylzxomi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bczafsyl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3atjkkasr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dhlktqti.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tqyomlcl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3sosuasoj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ibjzansg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tqfbuyss.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3unhemmnd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lixfpist.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rfffiqlg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kljwqogd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qghaptpi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mupjnbin.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3btatjrod.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lxofpwzr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jtyrfnzf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rnasqmil.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3eyjlvwpz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3watzsssn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fwqzboez.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nsichihi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3exxzspsa.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3syzekilk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcxtordk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfmgtyn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zjmotbgt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cebjqkwb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3udxfdsbs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lsyrjwib.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wefppdau.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hlwwdwqt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3piqkxhia.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ivzoloaf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vcjoctii.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pmyyjmoe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xtjoxlpx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhoqbjrn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3veaoqmmd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hpnrjscs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vxunaqil.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3curkowvv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3nossttpb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wmhkyylw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypblsgmw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3eevdkvty.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3enrfazcp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oweoxafj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xvojujft.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zrsriery.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hquqvipf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3hutinrnc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3grxntwde.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nsogwosx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nnlkokxx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3frutqeqv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vmyzecgx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ctsalpsy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rfsjijqm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fygyaove.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nyxrnufc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vodagmie.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3dxqqjxwo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3onwniyzc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kmhpxxtq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nfkizkwi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ugpbujwv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dxeftict.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vypzerdm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3iojkzcdg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ophhrhtk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3whyfkqkx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qqwplbxc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3apxtmcfj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3pvwpklcc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3thrlhdln.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rzbisisk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3nrubvffq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kliarjqe.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3owtobnrt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xxblshbs.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zqnfnwzf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3nkccijea.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ebntknog.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fxiwytdl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hsijxidl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mszzjqez.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wlbyyzig.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmlyifir.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kqldeivk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3palekksc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iuoigsuj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wyrymztt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wvolaued.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dnbliakg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3trnjepte.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ifvykmnl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ijxdwpov.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3eupkukxo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aswjlxod.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ttamiilu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3jioomxyo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkihpfxo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ccjclinp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uirsbmoh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3usyamhue.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zymygeae.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbalnt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vqtsqkvs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nayemfze.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3gmtwbedi.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ehazvuww.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sqvnhtpu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bpbyqwwp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3svgybwqx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3glufkyqk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tmlogsca.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bepgmdzw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3nbbmvqsc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnqbug.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3eyuzfdmb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xwhqlnni.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ypmpgiwx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3eltoxaqe.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ztoracqj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ayjunvnc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3nivrmjcc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ozsnojtf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3htytdkyo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tjxospzu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bbgllrcd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3shbswloq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xaffeddo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tnkitoct.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cpvbqeja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3klpnhjjz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bnwucotw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3dgymfnwd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3polqzrqz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wjeadigo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kcraagov.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3necslibb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tmyczxbn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3urysqocy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ksdffnlr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vgvvfqbp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fvxyeadh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3awphkbbx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3defcgutt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3riztafsv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3slpdvccu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3drdwmxyz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ykxiflxz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nsyxottn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rajzrxiz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3abnbiuoh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3sgwohxlc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3nzixgray.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uaeowtoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rlfdsprb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qnabgjso.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ocllfuzr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zpmzwhfm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kzgekmih.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zvamcxam.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3oqkiifnr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jyzyxlhz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dznnmere.html


<!-- 参考信息 -->