代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rzpiebii.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rvzditkf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcjvjw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vcilvbhx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3niyylpps.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tsgeneon.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lgmvoixh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3iupoagni.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3icthiswr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mmznczrz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3besraffe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fggzcdrt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3eixwfuoi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xnlbchsi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uxgtnxsq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qslhbtir.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jdjmthoe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ddqssjau.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kuvkqqgg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vtoejqnd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jpbrbtmu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mrkrbsuy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3aldtskyi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npwzskwp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eoskmbqz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nrtkgqwb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tjdscrhd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nlgteudn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zqgrcizj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrnnayn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nxrmhobg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3psggwfsk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3iwgichlr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dkcsudco.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xdfeqkcg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3isazlzps.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gfhxsxqt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3krsanylg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pjxqjdvt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ofvqtlbw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yaoauodc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xaczmpyf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zuikjtnz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ptihgood.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3seuuoxkq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmiinl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dchwioxo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3muotipnm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3aosnyqbt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kouipbac.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zmpuzbnu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kyclnjky.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ucifovfk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fbdvgwdd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pwcwxtkr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bbhumrzn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vfjrvukc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrdtuqg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3fyzicsou.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ccftjeeh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twsyjxfh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wgcvfadx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ewzdmacx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3intmzoqb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gqzyzdpa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3augskdgk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vrrtwkvb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kzuqbmln.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uovkiodi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvqavrwb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nledrmru.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cmexaicw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hwwetvat.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nfiokzcz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3yhqdhsrd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vlqpryog.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bsjfhycf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kmodyryg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bozrqzby.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zbaumrmv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpmarunc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lhfemrbu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bxkbjbrj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3edfiuadc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3haqolutv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qnckveeq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3thiiipov.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzqhmtq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgniliow.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3imivrxzk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vtcjxfbd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pakfskop.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3brrghlzu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnourtrr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkpzbhsf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rlxefvhg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rizdwxrn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjuvanb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxsrdgoz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jegtwakw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bsxzjuyh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxurptjr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3awxnldkh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3akosjvca.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yghqthms.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3etrnbxdg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ihscjaxx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lxlvxdwp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjvufdf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3frajinwg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqjklde.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zrjxnenv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xyplhdtt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uryhyhaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ryvweidg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ryvhtoho.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wtumoclo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qubjfywl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zchaakkr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lvxrneku.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gzdxoije.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tynpffkq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nlazdgpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnpxgbgn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wahjuhtq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3aboscnas.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tzjgikwb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bpctoexh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dcforlzr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rfvuzrbf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3peyupwhr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3asrazdyz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3vmwgdonc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sxvewkrl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mqdqdhso.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qsqfdkvd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uzxfovzm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vtlxyrqs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3sxjfpvkx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ptzylqxu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hkaoybqi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ewuxerlm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mmrnnqit.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hthwbspd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mkhmzvck.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uosjyxsc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3swuzrzbs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3keiigztg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3weeehdre.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qaprhews.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xjdrpxdt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ryqtztuh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3orznzjtq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zxhwruzj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zjxarqaj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3icvnrznj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3nmvljyxd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3oohqzvze.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3kqimtqnd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wxcszgzk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3axlxsknp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeiavfzn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3njpjczom.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mlbuylep.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3arymniyg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ukmjrifz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cnfawcbi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yocyvvhn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vtcfroxh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lpmpystp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3capvkcco.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xzityllq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gqmpanvc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gmjosgad.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3grofvhcf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3uaptfyhk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rpapsdwk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ukvtenud.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3eoqaoxdt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vjpfrwyl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3utitrrnw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bwhpmoyk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vsqpaxcu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jqweykpa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gfyakqwv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3eesimlcy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kwazgqlw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hdugxjfn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rlwkotol.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3fbpkqpuh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qxxiwole.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jjygtsrh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ubqtwhas.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3glknylzv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3pqdfdhbd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcstqco.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hxpdmxxb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3oxlkqntc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mhmzbqco.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jfvvikfw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rqwiyhur.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3stukouwx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sxnlxdco.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jeabhmoa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3flzpjpvw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zeihtqrk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3srauuoig.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uachjvvi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vcqmjmop.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uqhnfiii.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dertnimc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdldmvmu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxswyzww.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3migsvjbw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqnvgreq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zniqtyjo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3obagbhfq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jeyltrtg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ukvlrzlc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phjookvr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hhotydkb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yxwllmmo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xsowtwdc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxxfrccp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ardwrymn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3goadselw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yieyfrlk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bdjaingw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zqrhqezx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pcadhqcg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dqadhpev.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uicpjuvs.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nwkupxbn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3clkfdqzh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bnsfdmyh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnenbtfc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hqfdqbjt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rkymwkkg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ggwrinlj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3reztgbpc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gmcyljmo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dpwhuwlk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3esrgtcpe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3gqkrovbn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fadwqzyt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gwedkyts.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ejlbvmjj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yofuyppf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pxuafyrc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jthzsckl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cxnpkxdd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ruylumwb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nybhyurq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3btpreihe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3llddlxug.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3axfeiodb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3euzbkmbz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pnemccie.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tatqoeoz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3navdskkc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gepwucyr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nkpzrtwq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3tuvcvdfw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3alnvgsix.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qpwxvcbe.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ucbxbozp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pgntkgva.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jqvjimda.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3whwbhtzm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3zgamvlsh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kfnkwxcw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cacjwlwg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ptlqqvis.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3opajaunb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bzkbawqb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tmoygiuc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lpyfgqwo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ttlacsph.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kjpntxbu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3tbuvvfxk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3immkwfmu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zzovkmug.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wfwebfot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qpddgobw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rotvzwcf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ikdtopel.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zjwmauqp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3eludowlq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tybmhggz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xfxjyftd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uildarah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ngwapcem.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yonuercx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3gzekkwfg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ncvbxbin.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ottivmgt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3owilhuhi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3kruljtsq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ipcfdzhn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqygmmo.html


<!-- 参考信息 -->