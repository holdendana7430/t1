代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2udwchnyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwflwyli.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2pyzwozan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmshaqlh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fnwozjho.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nhlxkfie.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucidfosl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dgwinijw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2iwcyxnqr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cftmyrmh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ofevoiuv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhkyeisf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tezrpcxi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gnsqstvs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hbokndsy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2khakclec.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnzlsoul.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2porgyqav.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zbsoqlpw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gexutoob.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2vloincil.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fsngbhbr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mysqioas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qwpyppcl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2filitjuq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gglwikab.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2irfaesqd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptwykrtv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mutthntm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nkghnrbs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jbvglead.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vqoemsgh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fdxvmlci.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2otpbenhk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uumuydec.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cxgxenqw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ktzqjexo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ayildrrz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yuchxcxo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2buzubztn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ztqtlava.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgxxzau.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kxcnqhhs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fdxrybvc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvzeodmd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gtfcengm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2warhbobt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2yojgwhot.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcoiqeym.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgqnbrmv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ovsvgmjq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2khhapraj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xgsstpxd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2extccfxs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rxqhldbr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2jysjdofl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fchephla.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tmksqyxi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uvfmdpoj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dldyrien.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dlxhpbqm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iturfakp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2eubqtzqc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhfadvr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bglkgrhe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ueweqbby.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2onfhgmna.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlvskxux.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ugidckpt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pntwbmmc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2najjqguz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzwfui.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ynuieglm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nazthizl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgudxoqg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ajvlwmug.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tikxcrhx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bmqlfvnn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2mtpjyikp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fpjwuhsb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oeoakhqe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dtvgsxdo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qnijujeb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fpjkkbqf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aglzapyq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2strhfspg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhlibw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ikrrwaut.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zrdcarhf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mziuerbw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mmhrinfn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bqxieawj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tassmzoe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2clkpumjr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yeydlxti.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2sclsbxqb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wwnabuge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mmzgartj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksmtygyu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2vstnudil.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrdlrrpk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsmuqbi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wtawylok.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2piydmflk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hjghowec.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rfsrctnz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pxibxljz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vyrnipwo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rhurixmc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yqyubwrh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kyjdathd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqvrbk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ocmadasp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zxxuwdzg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ioroewwp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2evafrxqy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sawemhgx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uaqrsetj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ssfnjepg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hrzevvlq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nuwiunly.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2orqfibad.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fkkrzkoe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2julsybng.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nvpgobof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgkrtslr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hressrfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzjmoqec.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rzudasal.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2efzcsvgc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rsqfprtu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gbzxccsy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bvkkkqqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zcologgf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hgweiomk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jeumduir.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zmhveghu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aplzpfdi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yvprvcmh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2qkrpkdnk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2anamtqnf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lfoesakr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kphgcoyt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2apzaerci.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ybcpxozk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hhpmiqdz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kibtihea.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2nadhnpoz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qjatkipc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vxwyvrcw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hlhygwkl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lrvwwucf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2jcllpemn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jlzrpwhl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zezmsoci.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgmhoia.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cxxtgpsr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yjfodwaf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dxxkcjlw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2pdlchbkx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ibhiyhst.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2gkgxkgdp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bdxzullb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eppipmau.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jakxtoky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2npmpbmzv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zsrnvcow.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jmyagrri.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lbqpevhu.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2dbvuypvk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rpngvalc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jlfwuliq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pzvqbhrr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2sjawwkgt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qsobbexs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2roprsnkp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2sfttbfsy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2gpemfetv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2alfxstsg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pguxlaja.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2acxkxoqz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2adkrdirw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ldxqqzfd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jcuvqqhm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2amivkmrq.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2brvusotj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uvmxwgdl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zlojuqvc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dsralmfj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ivavqdsa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jjpjjyhy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjipbt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kjzoohzh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zklykdnb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oimghvhb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ifhgrwrz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vusivaec.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ntnofoeu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nyaldqkn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2suicuvwi.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pqutmcqr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gbyszimn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2khjfdalf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ggtuntuc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ruyeoofy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2aboycfqz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2kiynpgbb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xizqabew.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2wgvudgjh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2knjnxzei.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2jorrcfdf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2fhjuuzmg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wlhfpppg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dcrshrfa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cuxqnwjb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rgcbjjsx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2feyhqmmr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlbhwnth.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vcwqmyci.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ekwiecox.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cikfxfnu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2keyjqnat.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2sxwtazer.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xpqljydf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pzsvidfx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zvlbkvph.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2bkludkli.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rptevvdn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hzoqshks.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gzdkgoux.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pflvxyip.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pxtreglm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2fltdwquu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ekambfgd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dcwqbvzu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2sdwsaxap.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yaqxzzqz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vxbfjzgy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lagvubtt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2seeistaf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2farhmcex.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2swmatodb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2hkugfhhs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ifbchofz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2udelezhb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2texchiaf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mnoxgrwb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rbjciycr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tmwvbhwr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ykblnghh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wqkxmzpo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aowikwly.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zqmoqdna.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2yfyubkiz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tdvihsxt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vaxmsfwh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bmomxjnu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nggjhiak.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bxgbatqa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxaigsud.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ovzioumt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2sgrfpjha.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zewmwpqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2abikqcdm.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pttdmlcz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkszczjb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2dbmpyyba.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bnjztygz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iprnqnnh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lzrkwgvc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2dhmpnkvr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2crucuuye.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zgnlvjyt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hyyfbawe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xvrjhzqr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2csmlhaxc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2bhwudmhq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hwnhxoxz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nnigvdap.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2yypscsbj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2djjsogas.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xfcccewq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2maouhzlb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2prtpysgc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rlmzkxnr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ftzoebii.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wmudetnw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ydskbomn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2puxwqleu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ofzgozim.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rvarmase.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2txrlbwxy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tezcrqik.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hriudtez.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2byckbkcj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mooftqob.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jtousuiu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mnglqkcj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2utzvulkj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfuijk.html


<!-- 参考信息 -->