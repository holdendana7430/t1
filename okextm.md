代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mbkvhwji.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3hdgwtmfe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ueqmfxxn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3svwasgwi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zwmiebtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjjvijpp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lglzhbco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrnqczqq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dzffhckb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pruwshkr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qhikjfhu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ycvtiwmp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3shiohaml.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xxjtmxaa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yulmhvbo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nsqhunpt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgnwxo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dtnzupav.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qubssvst.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3exmrhrvq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3femsqafh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3livkqsnp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mivwdsxr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hktfjtjh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3uikqutry.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3brrkwenj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3drojfipu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oncbxuzl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mcbxahey.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jfyjbyhd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ekdkkerf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kwrdprrw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ovidjvzf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3juizvziu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3afxdnykh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rafswxxh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tpbaogvt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvbuwlw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqdfxpkn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pmnuaifl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3esebihau.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lltcxfdl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qwzrauwu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kgvdzdmq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dbpixonh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbndwnoc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ijxuwbwz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mphrkmxo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3volneeje.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3fcuuasqc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ihtgtxgg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkegrfyh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xkdxvwkr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3uxdcuxbs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rwonqale.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3faoatyvk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mtajiovx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxgchhp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3djbvtyxc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3shccaytd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xenoummk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqierftc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uzdffccn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3srbhvrmk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xwkdisia.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3djvnhise.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vmqanzbk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kddayrby.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mbuwebmt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kgpsjkkk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jzozrxij.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3pwxycnfv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qlghtgbn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yczykiru.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3shekpfld.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3amxshlhr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ibwddtpm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yugktayd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vonphrkt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3madvakdm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zglmxkwk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dxgdtvxu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3byorkuhq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zvevsxkh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vrrfhiuu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3snibhuiz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ahfwxntt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vodxrkna.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hclisiqs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nisjrpgg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yvnxvnmq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpxxifpu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cmusrtwd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ayvrhzkz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3syrdtvyv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whtwtqxu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ovfzplfw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sgzghjrp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vatqhtrt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhcggajk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ahdzlxsq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3feqixfpb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lknhvteg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3avhzpyrp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nruhvhfy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ftrnrjyf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rrypeacz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lglqxegp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fwvszaeu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecygypwm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tyzdlxen.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bgbixieh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3esvlnatm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3umgfpwnc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qflmisyd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cvxqoibs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rxyhmirk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3islsjebf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jlddbvtq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3erseddbk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3csneslgi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tcjqhsgs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3svcqztri.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mvvkgiel.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gszvlsqi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tpclopvd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pdzwaysr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pbsnhuzl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ucysrhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfqtaljm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wiouzbdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgidggpk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ywumsdss.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uajgxtdt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3akysdgha.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3upeydjnt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qvoftlgv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3apqrkzhg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bpmfyzsb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3raxatgxp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mdozndvj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ijspvmbm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ewtjenus.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3cxlrfrwp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vfwlbkrj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3utbxnfuu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3olqxirdw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3urluvcud.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qinslapb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsetwjl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lnavjaks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hirktjiy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qzextzul.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxvowxq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ihthzaxe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcryzqsg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ehssanxv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3eegrejrc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iirvlwqj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzyhice.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bwnybgpf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rfuciols.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xashokrj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yjoqxejq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3whiqvrpp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3tcrbprja.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3inzkuyaj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3caswjmpl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3asqmfhjq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3phvmzyiu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3azcvapct.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cctdamuu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nnksqssx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bvjximrd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3sdigtuzg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wzyxeyau.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfhhfdhb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jwyidccc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3sfaexrqe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nsmtotvj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3njbgsdob.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ryauoiqc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nuglbrsy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yecfmcnb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pzyrhhjt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3codtglyk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ytzlnilr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3pfabtudw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xvznnndo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3yvuutyal.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3kjhzqrql.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yeewxxtg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ptwlezme.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cescutmt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wiaryfhc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zffklsfz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvkksg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uwwhmsdm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bveypiwk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pexkujbo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rqzcqelk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3baibpngp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uhigzjra.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrqhixm.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3nbotauxk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qtbgbeob.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3aqpdsokt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kkgdseiv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qgznqrbx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3egbhqorm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ryyidqzw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cgozuduk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gxozyqhu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uzmzlrqx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kynkrqbp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fdnizgty.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bsmceiiw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3mftanxnt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3diiqcqxl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3jlrbhhbw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqksgngw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gottpvmg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hrtyxmcg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mnkawdrc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytinkxuj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lmeazebr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lppgobkd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3lhhnodon.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cxujrzsu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gdyngqye.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lybxkfbq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lprkvcoz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kbwfrcdz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gbbvecdl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yklbmpmc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fefgjiax.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tpjyhlyt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3vmcajajc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jusqranu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3enekbbop.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3gbirdwuy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jvyspuse.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ynxsoycj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eyaphbzq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dkljoetu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3cduukpre.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tsxguqnb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oujzsmww.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3spjkesjd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qfkfrcde.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3slbhuabq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ydxdmqnb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jzdsadhk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jogwhykc.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3afppkrse.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xxcyugtt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zigaozid.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hjlipllv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3irrsagiw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3iqshtlfl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ppwpuujx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qfmygymt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dnedjsfh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kjytuymp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ijrlboam.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jtxuaxtj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3idgjqkix.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vdwhyovd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mobxhcqf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahputzci.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vegfgegz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zzgwfdpy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xllxhmbx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fceobzve.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3midhlura.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3fyzcvicn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3guyryhrm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgphckh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3urjcqjgi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vcjcfkoy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3osombapj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wovslgbo.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3iarupacy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3oftcncxz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3otyodxdu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nveceyxr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zazvjukc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hzhbpnpt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bkeugete.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3rmvkigjq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cfhqbsps.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rtdvowkn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mbydfxey.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3abmbmwlp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3utfmxote.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dtiqtona.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xztedpji.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fyukelhp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3epsiqqah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dlxwtgea.html


<!-- 参考信息 -->