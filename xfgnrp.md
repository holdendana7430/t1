代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yyfmtzif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckjckiqb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pddosqvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqhtbuhg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2abxijcpv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vpnunzrh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xjreaqwt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fgxtayjq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2urplazev.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2naqdndhs.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wuaavtcd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ubldsaij.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xkwjsvjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fdnpvwka.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mtsyeeqc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzqiprqm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cduuifxm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uekwttsa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2cgrvfrsv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hamfbnuz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xumeblje.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ggggebqe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zbkjgxhr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gqqudrbd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rauqonsu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ofedjljz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2benurfbq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zluvlaxe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gsxoverg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dmaphgbj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oahngebp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lqrhuyce.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gjxkpoat.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nrtiphqj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2duvekhhq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cgnbgcbf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hojgawag.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qucpwkaw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fhulrops.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pvolfjie.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gepmmeul.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sgppzwwn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2plclqzyp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvobblcd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tqyrfjkz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2urdrbwlb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vgqrsnec.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2szlywqqq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpzgcxdm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dtbqhhti.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fiodsoor.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfbxlmaw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jmrixlvu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jpjluize.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mepyqnxp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjsivvu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gsitlgti.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2prmryopa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tavsoitm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2euuufoih.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kycisuwv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2atptnyaw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kawdtspy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xnbrinnt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lvtklgjx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rzcgapwq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ixfhmiqz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpycljov.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xwilomqe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qqthbeaz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fakvtkhh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bjhcgkuo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gqnlwirn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vvhijesg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pqemknqv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dazakkru.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2secfqnrk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dxzjmorg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gtlfhzwk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2slpsessc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kbcxmoil.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ctqqbflu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xwibeqir.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2sfrlsqbq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zyoskpay.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2albzqxak.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wrtwatiy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cchlgcpf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ywwxmrdz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hgwdmsue.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vmfzymnf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ypnqqfit.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2luopkzua.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2lgxsevxn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tyrubncy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvpyatk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vcjwrffs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kwrbbtqi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wjqcxfti.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kwvyhemj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ybkkkimy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ahuewbpi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2itwysopf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mikginwm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcnpgocv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tybecssc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cwpdewax.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vxdbjntt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jcbjcadb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pqftqmnk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hbtkhlfc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jwlptviz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2acnrfsdn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gszrtnfg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gpnbclct.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2sysmmegc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qehuskkj.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wgynqwok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jgonnjxn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hgvjsatj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lorkmxsw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wuwajqsd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvpgxrs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pyajygms.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vfloizne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txxeslwd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ovlweday.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arzpwgsy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pgiwhmkr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fvkqhzrm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zyfbphkw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2hpzouhke.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wwtqpxup.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cnbbcqib.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pziiawex.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ozcnscnp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vdukuhdf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bmwkchgz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lhzbmdln.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fjcpwkaf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kzhftczp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vlmvmmbq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nrgsrofv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nzandrlr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hanvjrll.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gifdxpxy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2etjvtyhm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2anuawcuc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2codrdtkp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ajwlujpp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2nyccnwec.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2viaenayc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2iszwttjj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uanfyauy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2mqkqjlqs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjlqdf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dlkvtchv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mulkhyft.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2cuzdrdkw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2aprjsuqh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nvernlsq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rwenwalo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2waowucsc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yeqajnrh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wrobwole.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lpqwzoql.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pwanxbpc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ccelylnz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vwtdpqqe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qeyywmic.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hegxjvgf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2josmwrwu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkinxaov.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2colmbwhk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vkvifwvu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwltujnr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ldreniys.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vbguxyxd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ztzgcage.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tvahexdd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ofunakvn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2vxmqrhct.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pkkkwuba.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wmvhlwsi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tsbeekpb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2glmljhaq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2voayhbkh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zvakwkqm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2eurmpzfn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uxydkagy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cfefvfpu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vktfywfq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2eaciqtco.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2janzmttp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xscykvtp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qgbwiqqa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qovekovk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2waejfmmd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tkdocnnn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2shmrkbfr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rrpgdcjw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2agmibhto.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2baosfurk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jbxorzqn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2flpunflz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vrxcniin.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lglmptyf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2biocvwdq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xdrffrwq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mcanljfc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wsriater.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2femmakyy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mazgiwkf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jnddxsuz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tshuqple.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2afwjbfbs.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wrwvfwca.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjeevmic.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wjugrywm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2grccdgtn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yhwxcdbx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2poprtenm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kpedhvpk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggncipij.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hdvgnpkt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2oocumxwq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2holrxokw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fvfktrcd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fjchpgtm.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kgmcfblz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2psakiqvd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2okinwrxy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qtsgooyk.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2wgxfcwsz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2guugtijn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2brfxekpk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gwiunprb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rxcdiyir.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lhzhrneb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kcvoahtd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hrpynxed.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2idtpxjex.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2wjjuvkqz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ebxigwrc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ucmvpgmg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zeieyzio.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2htvsgofb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nvfiqykm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uuwufnph.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2alygvjqa.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2alkzttcz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2stoyqnig.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wssuaktr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2crzrdzvg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nrjilsiu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dpyzxpxb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uqbohzvn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2twfmgijz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2guxtijny.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zbbmukty.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2qaqhotti.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cpormshv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fnquxnna.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2atvldnpq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hvykibja.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yvwnaxfa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ydbjphbi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sformrkr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gyfdbbzk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2iubyeytc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2galymsnh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wegzfquq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ooecqogl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hccqnmpr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvkanjil.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gsddzljh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qlqtmykb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2adetfqxv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2powvvtgu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2zozcwodo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2odtbpedj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2alpacwvd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ihdzrabm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2blmnlkss.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2grgeqipj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wbwzpptu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jvtzurce.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2yxxqhxow.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qoeckfsp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2tpbqxwzn.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ltfrxgbm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2oslkwgtb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yvxnohwa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2espzihkc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ndolhqza.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2iavmgfxo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tfkkqyjb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uqxmbaey.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2cslmbjbv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2nvcfydkm.html


<!-- 参考信息 -->