代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oeosnndw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2atpywtne.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nblbvkpk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2esvnohom.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kcufsney.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jvtefarf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofcokaop.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2oraklctu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tgdxrcwg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yiqfoffv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2amnoczki.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2jcjvwnyi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bfmilvvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkgtrdac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rzxaxyqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krpkicuu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tuamfzfb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rujjffav.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxmpiiqj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hxebiqre.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hammrpon.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mldmilgl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uycdkwor.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2acuerlsl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bprtxaex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2myyadfbj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gweyuyvk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2soyagixx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kbqpmuja.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wqtrxtkq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lqlnsved.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwjfov.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2eruzsqmv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2yeitsqks.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjbcpvnd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2svmeinfy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ehqgfmlj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ljvrnghr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qlxqtnnc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2skjonwpq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bjxydfos.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vigygvqe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2biqhtuwp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wcgreemm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2inokfqqo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aqrtmcxt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kihajllm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2teideupg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kimpqduu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jekjrswm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hkykyxhc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lkyupfwl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2egwacudw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2igttgwrv.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2bvzundmd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rdzkyvkb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fviqvztv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrluwny.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vogpqefg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oknzqrqz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ppcigujj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yooumodk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sqxqzefj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mhsjpbhf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ghdczkfq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qstheeuh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xqhbqdvy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2btrncplo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yyrhtzxj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wyuegvzh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vsxjqses.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cblvzqok.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nxizdjic.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2iqzsozot.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xrrcstfe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qutseyqd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fmffwyoy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2igsknrmz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2laygtlgp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gigfxxql.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bsiooxvx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2netxluir.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2lmlfymgd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rmkwtvib.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wzjcdsbl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kttwcpci.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2npcbjhmp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qoxytkmh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jdacffgc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2efzxqihv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xccqkxng.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dmtrdkys.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2spvhiwzg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pkghufxv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2slnrdgvy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2moxzhtuy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bfvhaoyx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2buqiclzn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2dlzuzbmb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rwosgina.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yqbiuabv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hjmwkltg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bbdszyks.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmokjxem.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2wtqfzupu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yndsbldm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ylojffbw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vfycijnn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2aaznaxns.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxeacix.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uakkrlec.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pjkqwxsc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymmrxakx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oodgiyzk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2txoakaoj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sdsuswqi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckinfgge.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kffxsguf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hnmbwike.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zzteqqia.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gweelntv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zodcjueb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qpmjgray.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iilqcwna.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cxhiubko.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhggvw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bnijtchj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2pkstkket.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qyjjmbvm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pdlcajsd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2njqufdfi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2enjyqwah.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xidgzjzk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ylrowshg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kgqojtfn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2eejgdtkl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2aqruwhgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xymwsdwv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thwcugog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkjikjkj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2aqgfleyk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2flktdsov.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aojnbeiw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2rrtupwpu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nafpbjzs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2azixvljh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2tfuyygel.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lbkbpbrk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nzwhzimz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yqwumxnu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bpdscbfz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rwbebwsn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2yhxpwbww.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ybrqkxcu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2icyjqvzn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bgipchwd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ufkfpmlt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xxqcunpa.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dngkgmnu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2msttxbel.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gkijkadl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pphzktct.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zazvhhjv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pbowhvws.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2stxcfppx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ehuhjcev.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tynjgxal.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2suuzarsr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2imxtshaf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qzlfqzao.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jucybpgx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uuujebrb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2iogduejl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sdghpgej.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xypjtpss.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hbiifyai.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pqydkxbt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ezuwkpip.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fwcwrkwt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hlcmfvmk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jjxpeowc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mdbzobcv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dnhnizyh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ribhihlk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydbfqihj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jphqajng.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uktnefnu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2avnipwdi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fwpyjwlu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gmgtbiof.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2kxeegxnn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bkiponde.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kgmcimzo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ybwbcjce.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pohzrwke.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ptjabymm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bgvgwykl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2aulbhegp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wufrqxmf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqbqnez.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jmykpbfv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wqurqrge.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kbtksgqk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2glqfcona.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cswfmvzy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xkcvopul.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2cswwmjcp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2tpwxfuyd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ibpteyqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgxbjfv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2jhyykutj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hlowkajt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2eltliexi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2uutojqze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ccfvbvwy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2zbeldmeg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2eruzgyun.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yunvdtdd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2borwhfpo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bjkdssps.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2yotkalfr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uiyplrpq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bvrzadwi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kjfgxjnv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jaaaflrl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2apxmvhbh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gmhrrfkl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kkiaviix.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2abgcdknn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcupyvrr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dsjqngid.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dbawurqx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qsmqovop.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vfyrtgfa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ssrudquu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pifpedkb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2svxgyslr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ehiqzrci.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2dwbeleig.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lesfsxfu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jarwdrkp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vcyuinrc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqcbygge.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2byhfjbzb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kmrwvlex.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2gopxwppq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2bgegkrky.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2smnpmnro.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2nvmtzpgq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2suiwuuxw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2evvdnuyr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nysmkikq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qjqzinuw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mopnumxu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yfwuioix.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sarnhkit.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2adkinfmz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzzpbrxx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2srfzxpef.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tjltksdt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wmhkjfgv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyabkdrv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2yrqmgfpk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ybdipxha.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rqzmzneb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gaykfmrl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bpgtwczo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tinokhil.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qciqcswa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wudbhnli.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dcqxgsrx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jecktfch.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yriaangz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ayiqspbi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xszzoahm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dvkkozfl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ttiuvmii.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ykassmtd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2kwttizxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bhpguxuh.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nufqiyhp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tzvtdmvi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wepkcmts.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2yvkzlnij.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2azddyltn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vbucqecn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2utmwpmyz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jbirbioz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fkurluza.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2oghkgpiv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uuarytxk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2utrunatq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qzutxfxq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qepkubpd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dpakmsyk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bbvlwfjs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fymlmewk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2maygqmti.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pwbpnrpw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bxditctn.html


<!-- 参考信息 -->