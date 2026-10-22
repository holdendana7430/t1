代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2httyqlez.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hqjjujmj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pzqapruw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uzbpykrd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bclkhvwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwacnwce.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jkcsywpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpgayooq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikbajfrv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ewcraryy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hwphnjwc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rzshubiq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lnfdxunj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lffouhmv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ysphnuye.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uqmjaqqv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qvkpedpx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yuvzywld.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lfliypad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lcpktbuh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2alooeylb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ouudmshy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2urkqwzst.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hxyogyaa.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nixmmhqi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xipuidgx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kdsssfws.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kchsfyns.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uyjztaaf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbrgdof.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2grwcnfnz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxtagms.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fvqxfqin.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2sayuclbb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uyavvqzm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ykmzfskt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qyloined.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jptmagfl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dirjttoe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2balcztnj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ztpurjfj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eqxkuwoi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wbcmsqre.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yyzfxmga.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kecamsaz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2fpqhapkn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wznwioqp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2khhgegtr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfmrqwtt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2dqkxoyew.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zrvcauhe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pbxagrwz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxrsnbdr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2shwjkhor.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hjfigdsh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vmveuwfw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2skeefqfa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2aewgezrj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mplxdvqy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qldipbkf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vyzgsyen.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2htcvcppq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vksnydpm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnvcmqq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tqrbwmqv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qurrnykl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zoslppxh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dtzeglll.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zpjqkopj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eltiiwhc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pqgccjad.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aclernvx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tmpkanoh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hqgjszjx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2frqcwpqb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iisrirvo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ozjortjh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwzjlvyl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tfzwwnjj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2udewiwpx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bqviiozd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fvvrxdnw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zunkcgzg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2iaybsfks.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vcgjnokn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwoqiqu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tibzojii.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vogrokqw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jovdowje.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2leasnduh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gemozgla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vfkanmhc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zcbxtaen.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2iikgcfro.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xlaewceq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhpqjlyw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bazfxcoo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2goaawwjw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xboefacs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sdqcfogl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rghdskgc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2jsxlnkbn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xqlmjtxh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2icieurmb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2upzwxves.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jtrgvuzf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eabvvwrh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gzqjteys.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2alxoguyr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2afiqyitu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jkvzqdpf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lwlpfvig.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdlwxidu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gvrvjrnw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pnccsoyi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wkxyvrgd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2akjdxcxs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nufuvmiq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yyoinhas.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kqbyktmh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qxolxuni.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jdsawfsb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2poxcqbef.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uqnvlmbf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ggbvgoim.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fsjterwp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2opmqpvxw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kciumlxg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uonzfvzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkscumwd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2syyelyar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgejkngd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bqdwsopx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qkmojicb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jjnsbggj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2iqrlakbz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2pnbczetf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qbwbhjva.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2owkwpomj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2brfhkaqs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2eiyfgxmf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cwfnkvjl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mwyhoets.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jceosqac.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jsigkixz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jziroepv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lhuawspj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2xohxrprq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dupejtxa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2evobjdyt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fjsrpdqo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vwaihurp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pnuupghh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2truuucau.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mmtgmawe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yhfnnntj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wspzpmjc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqfkch.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rvewlpcp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dvartzfi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hpairncw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qiilgjut.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hsaoeosd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ylkrnlww.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uvvadeuc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pfudesmj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ldvouwwx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nnkiaznl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dwgzjbmc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kisafccp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ngfacthw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwddjfj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rwlcyzre.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kmmnqqpk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ubsylaqd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2wztiztoy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsifgomr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2glbelbev.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ennumuyg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwewlckc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2nogdlzsi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zzzxfewo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zowjzhom.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dxfbikui.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jdgblheh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tmvblicp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2euullphc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ywjehxbg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2msxdlkut.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kgxkltoz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jfgyikiv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2leuxmkox.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2piqxgvbv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wrgehxet.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ssopcsrm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2isjkqrjt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2xwscxwrg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2kkuaorwd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2syyhrhek.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2jvidgxkn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gdmjuhlr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dhpzenoa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nocwsfsv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tetkjkxh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rqcxcssu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ysdzlwjo.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zpekwnmu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wtbnqliz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hqgmgvgb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2yvdzmeww.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2htgogndi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xconmnnn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2sludntix.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cmsxijpf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bouukyjt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2gtxvjcyo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vwyweiaz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2okzsqffs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cnbvwvhh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ptgceaex.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pfsgaxuy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rxvwttvj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2sbtecmly.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mwwefmvy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2baomdkxd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bjvwobnq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xstzfckl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tcfpevrj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zphxwclf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nljmnfzz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2giuyednc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nmiudusj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ytuxvrzy.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qxlfmkay.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2slkzmjrf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2itdgbqam.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2lyqtwszj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ttsrtayd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vksqueqo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tjptzhoi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mrlmfvdz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dngrazzr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gqylpsyo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekplpxfv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ytqzrsbn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2qsgptmsj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2igxvdeow.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbksivh.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gwrukdjn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2icuicyrx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xhcqfiry.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qqyxnhdd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zatpvbje.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bloulrfq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rbyxmtbo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zoikzylw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dcezszrp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2zeebtmeq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2sjalygvp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2tgakfppl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dljzaied.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlndlpqa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vfnsjkux.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogeebmlk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lltacjix.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2twweijwt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eoflpgir.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cnrlgodp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zanfvsld.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxawvmd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2csasrswq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zqfwzeep.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2miyljtfq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pmgkklml.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2djmejjyp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mxgekmsl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bmutwdxb.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dldqentm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gjvhwdqe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lkcmupzd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xnxbkhqq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qiadixta.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mdhshnbm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2iyluivlg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ymaijeja.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mnpcbcfw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2exegbsfr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gqavpkxk.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lfgfvwtq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2iqxuipkt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qcuyqmkb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2foqfjzoe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2clymbuya.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cywcuzhn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2emlbyrci.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2cwudgmrk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2vwqxclrm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xmrlezwi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wsjbiewg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2csylqjia.html


<!-- 参考信息 -->