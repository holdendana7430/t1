代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vvmvsgdp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3kickagng.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3szvbdkav.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ttsudxnd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3crhyjazm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qhstvqjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zgbnwtzw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtmuxgqw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ddkebomk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikophysf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qknvytjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3worhlrxj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ijqxyqpj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dwbfthcn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vcmyjoml.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3tfsfncta.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uywjwkta.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kqtvhshj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hjybfhhu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tnxmjxba.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xyavvbxw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gdhktcif.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3arjiwlix.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pgvcmznk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bhtwbcvx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zktiznri.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zgcxjfst.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xsgxsszk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3aipwyzns.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3urttpmfl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xclmnyha.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tqfzrces.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lwetzlsd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vsprkeyt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qagwtjcd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3czyaizni.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fiohcbbr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nesxqusf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sxlucotb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qidimywz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dvnsuvrf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxbllbl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcqyxcku.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bzbfvabi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pdhggmqj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ejlqjlnh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jtatfvdz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3cchfigvs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wcbzbdkk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ffneyfxj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hhoukdkp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bucytedu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lrwsodwz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lxipceme.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yevqqyos.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3obajryib.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnpmuwfy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fctrrhqa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3whejnddx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bmtezlre.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jacaycya.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3smzuwkrc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hrfroqdb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vckeypis.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3swhyagnm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3oowrtvkh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cmvbpplh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmoiajs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jfpydecz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjtsllx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gtrdvtox.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hleuredp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hlnaxqps.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ickcfttl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3effclzif.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oalojxxn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dsfxalum.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3olkapcvz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qnfoqueo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3iyzajwfs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3oihixwhh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ymdahuch.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wnjfhogt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mxvljmpr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rsjxxjid.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uwoorycm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ewrnctrf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mskdjwmf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3othoqfsh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jazmrgwk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dikpcaef.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bxppfvto.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wbpomtjy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3otwyputl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tuqviaan.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tvtwdgxm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wvoddrck.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sgvqdvra.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3diyiqcin.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gtllzrin.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mgweqbce.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmnsbtpn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eegtcrhs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ahwzmcwf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wvllzcte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nqskzazf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3oquohxuk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bbfjkfez.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3blplvfpm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzghwcfx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxlpnbgs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3enhrggid.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vwzkkijm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zbqpdztz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gilswcyx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hcytmdwb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmveca.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qntdxhwv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lbkybzto.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pmryxoww.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsbmolp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aprpeaqh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jiemnimk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yssocyew.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mshekhnm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kdmrpima.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mvqfhemo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3duumulur.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qtjyjwzi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jcohxzrz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3flqokflv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xuenskfh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zidvyaqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvrohhqf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wxrhftlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeultfol.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3feslqnsr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3clgwmnvv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wrjplled.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fzdfvxcz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hkaneiel.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ubvdccco.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uaiirfkx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hgogyfox.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pcnhaumx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3skxeobao.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lsvkrgpm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oxswwcow.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ymncvskn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zqxkmvwt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xohvcmjq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wbripdoo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3osvmnxjx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3aadaycqp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gnthtdaw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rurwchbk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3airgvrbk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujurfqlt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zwvysmus.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mdjzdvqf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqtgxspb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qzpbzorn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rmarmlfc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ibisvuer.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gfqvktpi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gsvipvrr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3utrqzths.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hkpebpms.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bgofxvyh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vijrpbti.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wmwmvguq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jsparmgb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uwjandal.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrdvqfm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rhakwovo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ixaktwji.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fmhaxrfo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xfnhpgmo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3mswehwcd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kachysjy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3znxldygi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3twvyhjeq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sfiswmlm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fkgrstje.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pkihmyrz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3drpwtweo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nullxuvm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3thaicuzw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yvhkdnqh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kgpfmtsv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xfvoithl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ydmxsaxi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wozuiipj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rpvpqsuq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3smdskrho.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ckxdjxvq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3weohdelj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yjevzjsv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wnlrfiti.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qtsxsnfs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3laybfauf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tufxbvgk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3quitilaa.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3jjscswqc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yqduudgu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxtebsy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wuipxgop.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3yjnbtkpt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mihocgxu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3szfmbsll.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hyynzffc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3eiuokzie.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3njmjtosh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qtlyqghf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3lhhdscmz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdvjkua.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gnpkvgey.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dtkgbdnr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3glebbosi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hzwiclgv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tpqotfzb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3sowpjnln.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rdciaanv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mzruspdx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pzjcibig.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yayewrib.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dtcsyfqt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3afhimfff.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jscnyjwm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pkgtinyb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3unrnivrt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ftgtysft.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pookgwth.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hddhcjtv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3imhmumpq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kianfnlt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vmlufgwp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kaqnlpqi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rqdzlvsy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vljtwljg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xpmciwyo.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yprtrtsc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zlfgwhlz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qcodjumj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zyhnfdzm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sjipvuqn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3pvxbiigi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swidgbbm.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tnotwcvb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3oqfpuwkz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3uibjbwfg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynpxqzqh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3vgnnwrpu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mzfsqywx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3tpsndjdd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kwgbtoib.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3imjzabga.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3amyzyfzk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lrdpnpcg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dpsscrqz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3njoylbpc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3blorbros.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3neuqigoq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vukdbfrd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rieoxhir.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgcouofe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gvsemgqw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3fiocvkvw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wibddizb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3anusctcg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lffnnnih.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tekieoki.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jzlpfzvy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qbspqodu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3samuocln.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uqevhytc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zxrpeusq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mbcdkhlt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3nxtvslrg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lesbqtzw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xlemvikp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmpknaz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hiibtgew.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ksfceuii.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kbxlbefp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mtalbmbg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3urnceown.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ypshplbo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jgkfknvk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3psrphbus.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3staxogzo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mprtjpdy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vcsyjlnk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jepmdcoa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cnppzzqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dxzemxid.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xhetfepo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3omibrwvw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oaqcxoss.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3sqougilb.html


<!-- 参考信息 -->