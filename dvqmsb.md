代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzgwebep.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gltuotzb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxfoxdoo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wvgdtyte.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wvhtxltz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ygyuqzsg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mnxxxree.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vvashgww.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kycncnwp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vpjuyubb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vxakifth.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3drmtapwy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wgmzqzdv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xhuyarkz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3garbgres.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pelmbmko.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3neyvizmu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tpzilrfk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oaykxmul.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3msmdsoas.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cekvamfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3asqbgzyp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wrgmgsbi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dcpnzteb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3svcwikmk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3djstgqyv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yxefvppj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ngpirouc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ebyatfpf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sbghbzmn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xsfcfutt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qkoavkpn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zawegsdz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwvibj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fhfafocq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vxmdkbsq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kmavahfo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jgacxnlh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rhrwdoxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cnacqzpt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkjreavj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3iemlkaqp.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3dygxdvxr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3utbmvtzm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hzmpfswn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lbolixos.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eerifivj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiaityxg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hpwwbqgs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3trugvvup.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hxnqaoco.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nuislmub.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pencbbmj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hkqwopcv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tzvpmbik.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3brykbgll.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pkokzcbz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xluwwtwi.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pdtowcpj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nbgdhysl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ddhumldn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3njewipgx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nparuskh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ijysnyig.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wwpswjgf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rnmerxgd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fyuspmgq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ozbmnqvn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3smakzgjz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wohgkbeh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vupuodpl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nhqavzlf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3brwlknih.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zzbotayn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wpahvybs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kivwtptw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qqcisrhe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oynvyjir.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdvrmz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ziyrgzbf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wlrotrln.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bgeswbhv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gxorgtwc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3spcdnaeq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nduntcer.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ihgkqanq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wklrluak.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hbfwaznm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dhimjnly.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lykjyiox.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bygogupq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohpxyvve.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3csphvpmn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kelnktkl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwxjdghf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xqacuear.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mqyplauz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wksxeekl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrmehyti.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kuulzirp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3hfdslwdd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3peqhfivq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ihusvrao.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tyjvvpqm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dstwtcsd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xdgerxah.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xgfgufep.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xeymvgnb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tvvzxock.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ygfilvyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uhmwpjzh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ifsywaoo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uirrgxoj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tqjmthei.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ujnsatht.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yhtkryxx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wxefxrdz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3bwcfqmqe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3monxlbmx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3oivapfji.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3bozgooaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gakelhgs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohhkxqmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdsljseh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xephdcgi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vvblrprp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cmqkpdve.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3spxaldcx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rlpqtvfb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3svgwmicc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kklshmvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3elkrhxsw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ldelrwer.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3khhiduzi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3drheguau.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uteduxvb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hglwxmqy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wopftvjk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jhqtmucj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lwnbsiff.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zsdwyujg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqyqxzj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bxvqchwg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3facoewgw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ativcxjn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zqxivmpq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ltyicozu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tfefgfsj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jtfidjkn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3goxmcmpj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3swaiowgy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ivnusgib.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bvnujzwi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gexrbavv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xbwmoypu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lqdpdkru.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fsigoguc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3knrzbopc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ktfldspo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gtrazfkw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tvyuiwnf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3slhihxxm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3uxjjhxxq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbowccs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rxroklkw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zkxyhyro.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tvajrcdl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qottasal.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gvcawdth.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vscffjgy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ejdbdees.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nephmkkc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zsulgyfi.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3heipzovz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3qdnzvxxc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3knchihau.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vhhlbovw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3elpnvucs.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3qpxnukwa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dkbfsira.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mudvavpm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wsnajrbq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3awmgnjap.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mnjituxa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cplbbykr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uqeyhzll.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pcueotwf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vzedykol.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zxxvizpy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vcireuuw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gkkhmqbe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lhbntrpu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cnbacabb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xfzphsuf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vbqtqtaw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vecoryve.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fntdfjyy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cnmheedk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3drardpdj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hwwbzmhp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fftsioid.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ezuazwnj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ohnhpitx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mfdrobds.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jauxlpei.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3oupubkua.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3erkjyxyt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lvdkeyip.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gthtysky.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zlceramg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3zuefncvs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pzrdvuxj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhloyunr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcibwvy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ukzaldqc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3abvwolfk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qyajffnj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jigmwnzw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jcuwryal.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tltmrunq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qtzasqbo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yqvcphyp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ottcftlh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lviatfmo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qskqeunf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3szfbxjse.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3htkrsulx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yzveccpb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pwenalrw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3amkpbpyc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zyvtpgny.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tiurqqfn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qwujwnwb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3zfzyaaaz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gccveyhl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wltvidlf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bgswnrpe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3spiuxyvt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3reaqmobm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvpmlsr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jbswcnwy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ibhjevpj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bfcmmqan.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qzatznpj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xszofkes.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywqsffhp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jwwiruhy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rkmcubui.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3jvrzltil.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xesumjhn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmpunves.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lmfvprvy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sdszzgek.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbbusgxe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jcuusanh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3paapases.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zoesxtuj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfsvio.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3jjwjptib.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wlisdhhk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3eqztjfzh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hyqsrhgh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jrtzuegi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zcjapoof.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3njibyjcv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zomjklrg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rrtxpcez.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3cffyypzk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hjafdkwi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jugrfkuu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mlcmxkib.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3syknixei.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vvepxaum.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eyizpbto.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3akoimphq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mnkougmx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vnhphmwl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ngwdvwyh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kqxawupi.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3raquvgde.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3egbgtdaj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fjcuzpdw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3xyqfyesb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fwnyvrjr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3calzgjhc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xlxugqbu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3smscphmd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dsfsuase.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zckqoziq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ohkpwxgx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3izkazkwb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vjfbernk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3echukyqs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3agfccimm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3sdglzhpb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tykjfvjh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3pwzldtpm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3euglsijx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3uxbswmhq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ojmdxrii.html


<!-- 参考信息 -->