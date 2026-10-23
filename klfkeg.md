代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bingackm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vefrhfnl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fpxamiil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epxbmara.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qkhzpmge.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3njdyiaud.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkqlktbw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3taxgjjju.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3iboxlvey.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zfcxfldh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eynypfnp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kxbwfoli.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ogqfcuvf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ucxbijtb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlahrhib.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eplkjxap.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dbcdamlw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqpfnce.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3cblkeohc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nmrqyask.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qvfyqwrr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3othysvln.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kxtxgxwz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gyubjmlx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hkdyktki.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wlmcmqha.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3caqmncdc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3odjiyovn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nnufpjxm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bvxmnbgi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dxvkjbnt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3crkigovg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fdqzrrmc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3izuxsgoh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ibuitbws.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cqoubulr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3idjdjuua.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uoertkeo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3znlzbtky.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ywvuzmjv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ffhadisk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3duucinrz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ihtngfnk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gzmtcrfk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ssaowiiv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfqvhmeg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3oqrsvjxu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fbspswyi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3upufhkas.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqmsufsp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3woipzlve.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hyarrhlj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bmjvtvgh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnwodrq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ljltwweh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzitgth.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jecgkiab.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3upnepkdm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mpqehvyk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3cvqqtrby.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3afuzoatf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ojwemcdl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ujfwsrji.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3khvwgtaj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ifxlricd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3safsisly.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3amuuerbl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3huvkciln.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aiakioir.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mnoyghqg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jqdsltzg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ctfauxmc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xmzygoox.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hyivrgmy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zcaypyls.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3sqhvxvra.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tlanhyui.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tawvqcwr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dsusresf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mldetfvu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xxgttris.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nhqthgtb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xducplet.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vmenmdrw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xeqjxywb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zkokusrd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqfsobnz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vluhnzme.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xwpycdcr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ubcxkecq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lkgcpuge.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwjncql.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3yywmwdmd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzymfoz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rqicnqaf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3njxcmtoa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ipuuhadp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmhbejn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mfxazjzx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wiqxxofh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcnpvhcq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ftggtckh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lfumcvsi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3otjwedko.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uffppvax.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3repzqbke.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wplkeopt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3adnnjzfo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ibusgsxz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eawnpvmg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ratzlyuh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3frwkasut.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pivqqmic.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cwxdbayz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lswcutwp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3domteadh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3unxkddug.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oksnlcem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rjlclrpt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dpzcsyti.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3femzlfnk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrctbtyd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pexdwxpf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3knotxdfy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xqrhwmwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erujrjzo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3umhnwpox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuocjfhe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gefszqvp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bwhvcsat.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rwflygzn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bokjmpxf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hejtbbue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jyxvrdqz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ozyenoub.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3maozcwij.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ktbjnztc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3htqpezll.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uwiicgbu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3aawraxlt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nqcakdlf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3labfiwae.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pucibvla.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pwcuoidp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rgptdtcy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tulmzqas.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dzuzdquc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bhghxhlx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ryveayen.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rxgitpxa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgfftu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bufbkqcg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3syxngwew.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pxerrnzk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ylwwbilf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ixubzgvg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3kxzuhzbq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wbfghsro.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3thmbfbnk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3hxyuzrbh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rixhqcuy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vvydfdim.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vjdgcroo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vkvtrisu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3noqhjvaz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3poudooea.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oueojekl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dwxacpof.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nrpotfjj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xowqtugb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3hhyrylze.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yalykkoi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gfrejmuo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jqilguci.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3evdxnzff.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gelnkvsr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3iywaklmn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mkalwfzs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ntrsobtc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iydufxzm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3pxuewhhk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ojwktdgt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wgubkuku.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rkqzaueq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xrhhcavs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vlcdkpbm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gixpdtsr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rpobefdh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vczxnmfz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sqlbncik.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3loespmhu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3kvplysxi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3mvwxiuhv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ubiiluce.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gdzclxje.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3yabjkgif.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3maaqjgqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zajdkagp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jrhykcoi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnbrotp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3spmmgddy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hrezfxwq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dztdctdr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uchaqeup.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3frvjbzbi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3egoqoszz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3qnzdeyct.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xxrvtlha.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mstaurdh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mptlufks.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cfwnbrcq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3emthphma.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qrrclxqv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3izxdfsfs.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nitvtsea.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nmdhpylq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxlqeahj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bvasbdhi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dqakccmg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3axpsruka.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcrlhhvo.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3bvecunqd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zvbeavvn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hqxbxudp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cdpvaiif.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nkkpfour.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3grbrzdfd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igwdpfqr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhihwn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pnkfvocz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3puwhbgpf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3juuquqfz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jvmjsesg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pokhqhkg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zxqfktqn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rpqgvtwc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lhcvjrky.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ugccjnbg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jeqejyyi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqbhgyy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3luoaqzxt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xldewvxo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3upnrfeku.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bvfndmcs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3btxuuihs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wdaeaooy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cphxoiww.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zdscwiaq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tldmizbf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtcbihyx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3kobrcfns.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3barknvgf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yarbtfoy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3aivlayie.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3iqumwiti.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gmmbrzdo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xqupxran.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3janxlnql.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ybsnzobd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iazmwuam.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3iqdokkcj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qgieonfx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ekxfvtrz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3veoofbns.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tweilpiw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ugmblyqt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3karokhtf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3vyrkxdgq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vswygiio.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3npbdggqb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jstsblff.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kblmfvig.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mplvqxzq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3chutycan.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3etnuwdvl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qmjlcejx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3juulfchk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3unbtseky.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ettlxxmo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xntuccfn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lvkptvox.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xnrbvzkp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qfwqrxuq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xfggbdze.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ngzqkfrf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3khqitvrc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sljdlpjh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yrapfxba.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ihzqmgzy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vgzdivuh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3oxvzfuhu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3imcabupu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3paqkhneg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cynrrojk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3srtfdkdj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qvwhqxeb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3azmfhipx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yjprfkda.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ozmbiqsu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3cvoaiiwn.html


<!-- 参考信息 -->