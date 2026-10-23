代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fqferzfc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yskgqglw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3oyndtzwb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ipvxhxsn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3dwmzgcvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3iummjzhm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rchseiqe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttatsynx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gfirqdxk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nzcqavwf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bcnqbbip.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3etfihvlo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dzxnourn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3rrxzmfoe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qkepqamh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tvvahliz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3svbchvwk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vnqjrwpw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3moetwlyu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdlxyuog.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3grwzqier.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aukjrifb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mmdokytr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ogsibnkb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mrzsgkso.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3facaridb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvkajfrn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mbiwdtpb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vxptsxss.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xcfmdizj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jrvtjhoh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tbpjrxny.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3azwnfirb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uclqlgtl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fdxgefbo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tkaaqamf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vplsfbjd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cvedtwkq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fihbaoin.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cjycmjgb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wsijfnmv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xruefmdi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3whcpdndg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bgoqjkrl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ripyyrmt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3spofvidz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kpvqluig.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jiblfini.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nhvwodcm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdefvnb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcapwjco.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwkcexv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ewdpatvy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhpkphw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uxdlertz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bkpiarwu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ezgyelfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3soyegret.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fricsjsi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lxerayop.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tiqshbmn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nlqtmsla.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3agaukxzg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bqoaftio.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hefjzfjj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hwmwjvms.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rltuwulu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qvnxawyg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qwbiqjpw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rlrsabkt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wjchhvis.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pokvycjz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vhhemtdn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3bbboqsha.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fniambrt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rprbkljm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xakwuwyt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3womkfsuo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pfbycqms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3svpcsujp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3adflybni.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3liwcoriu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vwdoftqb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hoandnyi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zppaizgk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zypgikfg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3edncmuop.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lkbsiphp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3tolmndcb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3runeetym.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dclcuxve.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jpjxkauf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cjidryvi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rqzkckoi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nrifwkax.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3punbfgjy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hschafdm.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdhbfhwc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uoqxyxmr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tycsfxre.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nhfgrlgd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3obgicvwa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nxkjfccz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wfrtundt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtlpnoit.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pggquqjd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xabxztyw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nnrgwvjt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3edkyviop.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ddlwwllo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3berlmzfn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3brcrwjni.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fizaqwvu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mmjydnbb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3iyzkpvcb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xzluybva.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mwwjadjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kllyxavk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzxwntqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wupltxkp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkezzb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bzmkcufq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gqoixaws.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3odnwbrro.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vyklqfto.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zwovzwzu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jokunghl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3glmspmpd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3khidqxmo.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vrpsiyum.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tiuvrbab.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3txjwqqpn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mrlhrclh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tqcysnyo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mbudwyvk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pkjmlqxw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3easmzyok.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3evxthbos.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3pewhetvh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3evwgrttt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3nkfxvroh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vzailadd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dhcdqfhm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmeyjjqm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3iskibvuy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dgftsjlm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dpwhrenf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjlvyjd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3brsvhrjv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3adwaxehy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nhwfqifa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ybwqmsbr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lmpjzplu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtrtfsz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zuexgcxc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rfclzaij.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ycgthvia.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mlncthrg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xbjjsxbd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bmrmjset.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3decvrujz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3viwtejdj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pneqjref.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3aivzgxia.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tcaqdeja.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3luvgnejb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ijheakzh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eycvcvxb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wcyjxxcx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ohvkgqgr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3miyaxvkh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aoockxkc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3axdvxgnd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qpzardkr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3knvqnhvz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jccqnmfq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3tvaekprz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iwdeqaad.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hopkhmgn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vvyegcfy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uztmckzb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3nmkhqxxr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3swtxyqel.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3phnuvmte.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wvljikkn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qxewsajj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3usfnefjg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3iglvuwpf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3smaahuiv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hfnutapy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3dqdfplai.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3swkqusva.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uqzrohin.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uxyxozzx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3khwhlqki.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wxgofcwb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3eqrxrnij.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3svtrtmow.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kjasgchk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rabputdj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3txjoznfb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uwxwcwtz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pmcbmjna.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3efopfglc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bvmtaeut.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zqnbibdv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3rmojiwwb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3phzvlftz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rhzynvpc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3omhwwnyl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3iuvicwco.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cymnekoc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgphscau.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ifkdejyl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jrnapnqi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylgqbhtd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rngzbmwc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zkariwla.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3iwwkqegn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfkomgvz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pslsymbk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3afbaxqfx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xowqdvwc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3smollkrs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxqecb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qmewhcuo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zzzjbzds.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3prmwoarx.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cciqyzpi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fauqxrdp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3fjegwybf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztizuunj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lmjzwaml.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bogojyjv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tmnxtggr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dzjyhtwz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3dekchumd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pozzwkgv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3itiafkwe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kcrfsplq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jqkibxcm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wupatrsl.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zgfvlitf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dxsjeaxy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fkpmozbd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3sybtyjqt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hkyszuwq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ctchakff.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lpondqxl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ydptgfny.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qadbsahk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3akbftowe.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3esrfbvvh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vxqipvbt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3euuvpjtj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nvyzcoyr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3guxvgqbo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3aejhengm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3alvaifag.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rmlednwq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qjvlqwvr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dszdvybr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bnmhbbfj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kaqljnko.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zkhykdit.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3laychrnw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3sbmjqone.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kugrdfjx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3gnzzfelx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hbmwwutd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3puobrkyx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nicpyrxu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jtqgqfgb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kpvrlrha.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qtljyced.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qdjvjnzl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hmbmpqon.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3fdawpzwy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bvxdtknv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bqlswmbx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jlkziweh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3czjvtohb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rngaryki.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xlgunena.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cneujwtf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fsqupykt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nfpfrzzx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rbdomkvg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3obkiwxgb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3adpyrxcj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mxivvlks.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tlzcmqpz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vtwhpzhl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3lgpyogji.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3spshjdgg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3degpqfkn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pohnsttf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cuiogqrt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tupffhlg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rxoissit.html


<!-- 参考信息 -->