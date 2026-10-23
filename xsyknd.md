代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yiwwairs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlzwcpur.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mkggjefp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brmrbtbk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3obqjsino.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gnrmwles.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbnzemiq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xvrvijdz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vyvcjrrc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gwjrucfx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ktshtyiv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ibtrkjjb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fqnzjaep.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qeywjnku.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vzkpdrbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yjcmqvrk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sezsvyri.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3htgfzksd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3sexxspyx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hapofvke.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcapugjn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pigsgevi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ivmwwtcj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3edeahspp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fhkobkqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpaytva.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ekntsvro.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yavpksfo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vvhmtlck.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lyhyrdgh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbseilbt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3icmoktoj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3eyjizmjo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qyysdfjw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ktosekaj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywhiynct.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zeovyamx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uffmdcun.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3miiegqgp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3egwzrhgg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cbwjuves.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3uetavxam.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zitzdxtb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwagmlhn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jjjsdpkb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kycwmxdr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3adkonxro.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aafzmmhs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kqostwqp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgyprrn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hgufhxsf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3agzdmkww.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vptzeqiv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jvuowdet.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aslapzlh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ynjxremq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ufcjeqap.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wolwxncx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uugflrbe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3mjgeajbk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sxcuihxh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlwuina.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3jbhdamlp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pnqgnaiv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bwclgnmn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jhxwuxmr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nsqgwzql.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rslwyhnt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rchiiafu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jbywdfce.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ibzplvwc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zkqheyio.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lifrskxf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nwyypwzt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iwautqbk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3tenmjjfx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zcgcgpkv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jypnihql.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ugkzenoa.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nwdmotry.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ljlrsxzz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bkyxvwkc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ucrlifbe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bvqpsnnk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kjmimxvv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xfportja.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eduarlad.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gjgnpsmx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdziza.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ofsomhwt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tmjrnnif.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxcahkez.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3onaqzqnd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzxkfbs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jtqwxoem.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tcfvfgok.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kemaidym.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rexkygsn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xdpfxyyt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ezeqrldg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3uyglnkgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pkefhgmp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ycrokluv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3imuihyqt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xffpzkew.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vxifqyvi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uacaaxqa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3udcbtheq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nzzuqpsr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nmkuedoo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kpwqevkp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ysyxrjen.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xykolqpt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vtvynjpi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxavgzcz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mhumerzw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mhioqtmu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pegootvq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qvbijnbz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hjsxnttc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xtkwwwck.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jzmnlgnp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iwetfbou.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mgaezucs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3chvajqjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhskstgo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3riqqmvtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noxkhurf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yrvshvxm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3djggatom.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kclirobr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3muveewac.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3izptjdfn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xzwbezes.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqpxxc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ivnijxsd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lgymihgo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zydwhrql.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ifzlospb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3strfbkog.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vwnwlium.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3egofnwlw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ezjmvhdv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hfoxview.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jlbqkire.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xrsesffo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uqzgeftt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kxukftcu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wxyvhbpo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahofkjgh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ymetzgat.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eyokctoz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wkgbhxfp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxttakn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mvyzpdbs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pviklnby.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bceregsb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bvptvsnp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fdmspchy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lberprhx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vhrlcnpc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3elvfhcjb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ejnpyqqb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zahqpibg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3afmgfvde.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yccyepnc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rlrdylbj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3adrjldmg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tgecqjpd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3edrcznpw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3okezhzsf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sqywrbib.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sigpfekx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tkkhtdlr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3evogcixx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ppgfuuol.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3karvogkc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ftfyyjrc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3woqezhgr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tcelylmq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lfdtelgq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tfvhfvre.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xcdzhkvg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xkcbborh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ctxbnuqa.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vyvbbhva.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zxbpcozr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ydupomuy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nqufinlm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vcxslyrl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uoidfvur.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ootoymvu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yjynecxc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dwqlrscd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cgldegen.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3grfrdtnf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eclehqsp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vlyahxmh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cfymysmt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ppdbsxjn.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fykizkkn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jrnlcbmh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mddnqxbd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ybelmwle.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zrkiqqvt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xtzetgvp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lprchifv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgitepge.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bltupztd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wmhgcbbp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xypgxmxy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubavxrtc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rlmtpyya.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lanoopog.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cotuemzq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iceqqmzx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gamthdty.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxdkgnad.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqmlmldv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yntorakd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjztxjki.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3iwaoauur.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zogzmbyn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjjychb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gaksaqcm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ftcvdfcj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3oixhmzys.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ornfpixg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dpyeoupi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ilzpxqdf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mtjdyati.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ebooejuf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3twmvxtpg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dezeoymd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qfynjkiu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3gcaaxuyq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vgtkgxac.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wiwgtqtr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3sognisnp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awzmmqmm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3inypapaa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3zjfvzeoz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xamnpvgk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvayvdhl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dvoglnlg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xdqxzzow.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pfqarkfr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxhuoqcp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ywsivpya.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmbpboml.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xeyjzggs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mzhuxxdg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xrinenyh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3nxksyenz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eolpxawt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3pvniuejv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3njncmgap.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kfwvhcra.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zxkgmzrj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kpswzdwd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dtzozbcq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3azhcmyue.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sqcjcufu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3fmdiyupc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3yfisuuyv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3etlpdwzm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3msrhzdxn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sezmzbow.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uyrljxuy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dqcexxil.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ibgypvne.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3lclorelj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gnpumsux.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3azwjdtom.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ynyjbewd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3juvhjqkn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wsgqvhds.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tlxxnszn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3agaheztr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3eszbgqnj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3igyclvya.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hqwszksr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mxogpnjw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ujnfjyyf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mkkmuuvr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mpzgpnsy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pkkfgqlk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pcfsycqh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3woopweay.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zfuegptx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bwfmzrxm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hfrjseye.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kbzqvakb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3mhabfspn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mworyiek.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qoesdjwb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bdnshzbz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pndozegq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qwbmyccd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rgpnrfuj.html


<!-- 参考信息 -->