代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqjtdgyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pilcjlre.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lygpvkzs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kapqeiir.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ofqdfoog.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dutziujm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vkuycanu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3baukgnnx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnfraqgt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3grawefkz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lkzzrwoo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yessvdqp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uyuwcbio.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjwsqts.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ubuaymkh.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afzrohgm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xnrprgio.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xcjwnayz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gyojbbcm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yncrqota.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3daebjhrm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ngjpsfhg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbyjmofb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jmtpunjl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ybpvgrpm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxaaivbd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kodzywko.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ooghdbth.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mzpxuaye.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdnpkau.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hydkzsfn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3otnsydce.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wzenoqyw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3yurvahrf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3limiyymk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fqbsnifl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rdsahmkm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qrtuhzje.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3drgskkrr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3blzhowxp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3flzqgqka.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3bnoyzipi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lpfejpvi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fperkuma.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vmlssxyw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlvpelgl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mdhznlqr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cjalwbnw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zrifckqr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ifrdimvj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nmsjxlep.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jjrztevv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3blgkwyyd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lmsffzgt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3macxuxpa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zexcarln.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mclksvvy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pdhrdgfr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rhkylitw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3morcguwe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dhwaquvh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nthwpwfj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ohgwytvw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3gmyyxirs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tapeaksj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mezyrggv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3llqhdwcq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gqvwjfud.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ropgqbwi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uofszjxq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ujtlcqci.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jjugznpg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wzihcslz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ciyscrsl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uvyivwzw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nfxpkesv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fbjmyuwj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fopjszbd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wvbofbpw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ykwdjens.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xwpufczh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxbyxelg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wsxgffdt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yemtqbtq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3odiexnqw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3csxdeisn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqbewkah.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fqpompus.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kmwjzwya.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypyjwwhq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqpgzajn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dgxncypp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3tjhbifwx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tibjcqqk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bnhckznz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejywzysl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlqzymvq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vtebnwiu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eobigfwm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vebcvuov.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fectcavl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dlzskncj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzrlbhm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nffqjnnj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3abibhpbw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ixlvllxq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbwqjio.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zrxtrhms.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dfqmyhph.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jluoebrx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3awllvnqb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zfgxhzmd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tukcpbkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlibbcqe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ckjqvaut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhuitigb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aqnsrcsz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lyustuyk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3txqkrnwf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aivgstxv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bgrbquyo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qdkbwjha.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3boldzmtz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nhowmkce.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3owngkcif.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zomfavfx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mnqodjzj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bcwugnbp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3klhqgseq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gjwgarvt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3didcblgg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3krvhxybm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zmiekvrq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bqxhsdac.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3shrvyhlj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aaifikvy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ukrzcnxu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3peduhrjz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xzhjpdpi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnylqmjv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bhdshlch.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3nmpzboju.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3mxirgfgi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3epaocaqq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ynhpucjy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kutgsyuy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sjsnijkv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ueiwfxuk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3emmqanmo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3tskgivim.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cftmdarn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rjqpuvgv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gfrmecvs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrsqlcg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pxbkrsde.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wygfjkwu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ibpykmve.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3scmviqqu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gckippwk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3huzzveip.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mfdpshwq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xfxyuupf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ptesclhs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dnbftlnp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ogvzegqr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbduftm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gsxnvubn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3legwzyjw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nvmzholw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kjiimeno.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ovpdywul.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3esmhiqjz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zwkqqzbd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ebnmojbk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3irihweow.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3szwxvfzy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3quntgcpd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3pjhcwjey.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yqrqkzec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ulbmuakx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sddgxxrv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kzqfstwm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hgbtejou.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3vdddwphb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kgglwcth.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3loxbdrmv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gulhmadb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qwxgxiip.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3sphfvlbr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ecbwowgd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kaspmyin.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jwpcnbik.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rbjotdzp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3sneeghzb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ooudldke.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpjsbnz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lglnovcv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rurvsmwe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tvmiwdqn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rjvereqv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ybywaqgq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ikatcidy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3neblnrwh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ucfqltkz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3eqzuramt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikexnnaw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hgjcylwy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pfoinyam.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xspluqxb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xrsvyrzt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jjwpxroq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3iesycquw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zshctqox.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ypnnnkah.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jkxzpgmp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jmlmhbxb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3haoyoxkv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3tfsbidrr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ykreslgd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3forpznqw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rgvheafv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fezazjxc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fqvwtgwk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fdqgjizy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jfhfgudp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qvsqaiby.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3amtlxdew.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqofvfmb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rapwwpee.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bwgjtuir.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xjfbogns.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xlymkxkq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3znoanjeb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sqrmvbxa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pcfntxze.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yicituuv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eeedrsea.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvaongs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pgfjtmcl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3vbpmzpzu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3kseqalzx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3frtxdsgy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pfbidcgs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jgrhauyk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ekizftvy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ysflscpf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tuplgvoc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aoofskzg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dnsdmfon.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cqqbhxvg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3drbrpbjg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nbmgejjl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jnsqmpnl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3grqmueyq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3iwircztt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sjkamwwb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3moerpnyn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvvqtxv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wshuddgv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3idjtmkbn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3myxeosbi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3srdscgrn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iulvysxq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ntqrjnjp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3opingijt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3utsfuqup.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iydeoiid.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zutsfmxj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3djlhsncl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ixjxkuvs.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hgjylvqd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uwnllkep.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3yuvzvbnh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cthykfxc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mcizrmwh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3olanunab.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zqihgarl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tcebsszr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3medmgcok.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gbyixkbk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3wvooacbx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ukkewcjl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tdwglvfn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3dtxarbpc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sfbbpelu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3feyxvzkc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bauesmsz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3xgtjfuwb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pwfapwtm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zmlvttrn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mgxkihtn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzstkin.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kncifjwi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mdrkxtzc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sggtmmjg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yllsjxwq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ggpelpnq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zxinmtwh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ymvqhpld.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjqwwvfv.html


<!-- 参考信息 -->