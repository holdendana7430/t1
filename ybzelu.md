代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2amrwzvhv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nigkfezg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zzqnvkhn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uncfawqh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2hjrdhwfs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zsylhfiu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2yevacicx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zmpgdusm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aditjadp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agyyoobd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rezxenib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfsrevsz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2girjbdrb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ituajcll.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wgormxkk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wrgbrvih.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qlnvuhkp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ruucwynb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ipmjrkbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2glutnywl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2orshpzao.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hmyoqdob.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nsiplojr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vqkhfymn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2awqragje.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2crxxbcbu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2khpocpof.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2awvazwlv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2jnclrmzn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2klpwezda.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgohswxu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mpzykuzv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ccytynhc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cowoyyds.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ygejzfit.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vhlgivjn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2upxxpmtq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iftoejln.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ffveltuv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oegttrgd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vkdlghtj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2onfjduie.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xoivdqco.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lcwgsikk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ykyqzvbq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hgfgoaap.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nqculhss.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gnjpkdix.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ezrkoqbg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tzwavkyj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ekbvyoah.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2npotvizs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zutqeedg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tqszaqxl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2hcreekrl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ohgktwxv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uzzktyhe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mlplxcow.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2edykirld.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wrtyemff.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2gttyaerd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ztjdecwv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2frbiqaxr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2deqgviui.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dwlhmvls.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vpelmbuh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2sebmbfmu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2blwxehcc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2spgosdih.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rkljhvwj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gskylxbj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wavpgkid.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kufallhj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fepodnwp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nxqklsht.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2izxbdujy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2guvfzayj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yqruyjnt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ujsohwix.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tferdrgk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pcjldxoo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kipcwkuy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbahsjkx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aetoweih.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kxguouii.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qkzqquds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jtjmxlij.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2afokxymk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vacrouhq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jlqipjlb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fchouqdf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wtdemvqm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2udisicxd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sjviivum.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pvnvwfbb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2takrmcjw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wjyjtyns.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lvsdzftn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yyazyfge.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmfitcql.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2nqnlpiwq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjpbbzzt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wbicjtzd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulydhhpu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2auhwgoti.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfjpmkso.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gomqgast.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lopfjbxw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gicogfpx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lgguoods.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wncsblal.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2snccmlmt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2snsrovrw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hlchxbut.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vmhdvmqp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yfuqvpow.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lktcbqhj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jbhaynox.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vrdppeql.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uvqksyjp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rizfqxar.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yupeuhjp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ibttizab.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2axbfxbcu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2evbwpfsu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pislajty.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2irvwprql.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wnyfbdvt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovejxncp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lxjknleg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjrrdvr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ekgabxvy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jvqglnnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdndhhsd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ijmookks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szcpovtu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fpmlxpom.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2exipcmxm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mwjjbqpn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2edjsoklf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2txisxmbe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2vnhnndec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nnzhipkb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gxswufry.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ejxztuhg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2laacnwrt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lycyvbbr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ucirvaup.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gblfbhyn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bqkoqklt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lsxsbaey.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mamyennw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lealwtzx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ryrxdadz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mfcecstp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ezudpofv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qjldirus.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhowzfn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lwoyqvbr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzppiyjl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hanqgcvy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bkqnfvdv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gyinomed.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lpgqvhxz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qbtcxwyy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iuhrchgn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ckflfnze.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2iaxtmohb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2avvbxcry.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2prhjepii.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2krkwxdms.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yuihgqmy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tkvnyado.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqhnone.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2woimluyj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2cubrnuik.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2akddrbsk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gvkymsit.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2oenkxfri.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2stnijidq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcwthrhr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sjgwwhbb.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jduxygwq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tivbygqm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ndretgvh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yyhyxyuq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wtbzyftg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmjjgrk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2taqzkecr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2judfkfms.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tyiqndqn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2bcfabgkq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hzwvwvqj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nsmsdzuq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2devytqko.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2winloshf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2umojftfc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tvcgjfsb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ixampdeh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rcmqzrdx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nvhwssiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ackvscca.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ohhpdccd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nawubfne.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hkaoqmuy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yfeytqnt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2frzswzqm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2sxulilqu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2trkabxku.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xfltyefr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2izdykhws.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pwzmgxjz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2wxrhxqnw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ihswcujl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qnboedek.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyztpmts.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ztmddjts.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hgekevts.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vlgxpogi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2chmtdgfl.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2pzapmkfj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2axfjyidt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxraygav.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kunwiker.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpzjmkkp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqowmbcm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pukrvyxu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gjtonzut.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2svexstor.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fzneeldg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xybjgrrd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvmsljj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kudihabl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2yaqemhnr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pggobpoh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xevnfluw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vxxaamgg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cwqfdkeb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oftsuavt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zlwsvqtf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rthzexhf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2oszhvsrw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fejpzmob.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2drmosmah.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wwajqdds.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2paykwwhp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwthvigv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxjzqwd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ohdsknsl.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2efwwqdlg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bwodjvcm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eptcqexz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckpzrori.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nbqvyatc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jgxjxeea.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2prswqgaq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qwjulqft.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gcrwiwro.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fktpnrdr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2seagyzuk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mnfbimln.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lshbqydy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbrspvxt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lhcknsne.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iubfnzvn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfwaivbq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wfiixpwc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2asxwnccq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2iezijyha.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gfdtavup.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ejjjlfcg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aljtrfdm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tkmyqrwr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yyhglyvt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gaovseyv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ltghtrdx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wxavvsly.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qyrtdtel.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xuuiltsm.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pygxycsa.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2unmffwmr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gxtntmat.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fumbsjrl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2izipgjwk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pujidwzt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bvrtntxd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lplreshu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wabvwghu.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2spssxzfi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2eyrjorpo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mxnqgnsq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2oacuxyib.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ianallmx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nauacuwr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nqsqrjxd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2stofxsco.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lufahgxr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2clbtmwhj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fbreazui.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2jkiporor.html


<!-- 参考信息 -->