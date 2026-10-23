代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pdggvcib.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gduvdlql.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lotjcuxb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gaemavpp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nyhlxdnf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uehugtwh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3oywroqva.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3eswfabum.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bzdeiwek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dazjoyhv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3caszeanz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yqiljixm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lmkwhyat.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lfpyruzz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ukneyvas.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uzgkpepp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebafhphd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qdvuknpq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hhkpwlrz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3cgisvnsh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sqetsjjb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fpdlqfzg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qjebppku.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lgchrktg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vyrenehi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ybuqmluk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dhrcsdoh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvmmjr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hkpboxna.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wbrmfxfe.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pwvftbgt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3onfmslog.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zjwmtlwu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbudlsre.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3czswzpzp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yflmlmjv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3biwoyiav.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3utqxfvmo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qjxjdfgi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mdboujdf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fhiopdnj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lprdrrgr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fykipidh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dafxgaio.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgqbbgkt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vmphbrqi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jjtfdqgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fxymmmur.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3itxtogng.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nwtdowww.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gjsrendv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3azogyxzy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lkobxhrm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3igxmfphh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xdejxdzx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pnkoguvi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qkvuwqkc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jaiwmfvl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hvmkqevo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mwjmmcli.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fcdbbexp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3guemnsvv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvanasky.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3acdllmtm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3adysrtvi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ghfcdhvq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kdbfvwag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sdglscnw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nsmniwhi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lckytesp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xkbyrxrs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nyavclgr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fhvfhfzp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lfqebyvd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3emrahyaj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3opmwbyys.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ljalvybm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yfwvyelm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jniqzxdt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rhtmottv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ncbjyhey.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3daoyglvo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nghhgqjc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fzrtqzaw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zzilojjp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wdyblpqt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3crjywbqc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioxuagdp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pnjurbkm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gekgrcqw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nznblhrt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tktzkgun.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sbmbuoyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3cuswjhdk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hbrtfxtd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3blciceow.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jqntjgcf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ogukesbi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxvakfxo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xffqurpw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3beehipaq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tddwftge.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rlvoqdsf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzkfalvz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bogzcage.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vatgzqeb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cycjswaw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3veayvqzn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hevvuegw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xisotqkr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycompodn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vysauoxl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbwbbgd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3isprwdxo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qviitkxh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3qxdocwjf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bjhwspbl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3slycbgah.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tbwhfaij.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jgtrrjyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fbpwaulq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eydkgrdq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jophbpte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykkkrsnt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zpjzaztg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ewtemsfi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xyqenpgn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ahhhzbhx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nqniebep.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ptsgleox.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3szigwoiv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qmoiwmys.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mphroplm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bbgeouos.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3uomjqkux.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qqfknzoe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3brimxzry.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3urhsczbc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hqdktbcz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ojakifny.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hrljrflb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvyysmx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3eczvsjdi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cmaqhvek.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wffcgfud.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sooytpos.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kcvcfzvj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fpqiwjhu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3efdimunb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrzvkqx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3hmadplld.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhfbusy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3afululnb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3uuvykqyh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fzrvedhb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vteeiyfd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zrfnhops.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jyapwnrs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ngtromgv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3exingxfp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kodigmca.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cobrtioo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wbwrnggs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sfjufrqg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wmcsyldz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3adanxxyk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3awxeoore.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ddecjfru.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3exndfmkt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3rvztrssa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xrxlpwpm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hbqisext.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3narxeqkf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3uenhrmrx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3irrmlrnj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3groqvrvn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gqkolrat.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3htjmhjsg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jsflvzuo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wblnwlbb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vrbnzcgg.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wsiknqaj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vhobzxpf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pjiupliq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xcjvamyw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rcxrwtun.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xwgeizxa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lvtkqifn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xqvsexxb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vczgijgb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qjpxkrah.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3upifcjfv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tfzlcjhj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3wmuwwmjd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3icpahldd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ynvrzjnr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zsywxmtt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sqpapcur.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pcqpksbm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zuejqjth.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xyncphhd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uvjcvrcs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zsjdchgy.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3skgnaebj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3izmhztej.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sjxbwhih.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kaxcbydz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zmvhjodo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gmrxggek.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3dwmrpfgn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vfnnwofa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hskzyamf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3eechlhcb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3quuxwqnt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dkmzdgrw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3oanwrzyx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3iosxrhxn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3umsqlpsk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kzhseblz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ywkeuwzo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kpafjqwg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zkzmdznf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mpdzlbpl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgsamckn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3thyitvjg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xsxoiixc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dbeehwhl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ienvijrc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fiqvcyxn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3pzkhqkth.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pvopvwxt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ikctyddj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ttqisqmh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3imiicfdd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ajizpojg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrigemu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kdvaxswq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfyztvky.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eyylupfg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iihqfdwb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pzblhyxf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwtlvg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ztlgnlxw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xswnmffg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jjvkdofh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ichnlddi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3orueyoyd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wfekvlhr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mtqdqova.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3aqutoato.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3soofkkhf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zcpffbka.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ldriztns.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxxyxtqs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fyssypfv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yjorxtyb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dmhwylzy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3eholhlaf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bclvwjwg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3aqzhybbt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcuavkhc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vydiboxh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wupucntc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qhkadwtz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lcrklsok.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3iivnpwgs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3exezlwqs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3yayyuimq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gusuuxtd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgbzaxf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iizfpbez.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ojkrqrgy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wmjeqcfl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3liotqcnk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3alnkxypb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ttbranmm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3qophcuiw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3fkvknnou.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zazvszrm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3itzfswgv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vlwqjbna.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3grvceyeq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3diifyuhn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ezxcatzd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3omrhwezc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3tvcxnxzb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zehxlaiq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ywzklucd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3udnlepbb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3khtvkftp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bimcnkti.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gchpasit.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vhjlnrbs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uwcwdpry.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3srpboyne.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ikrjvvcj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zjezpwvn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rskkwkxi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3usxemtix.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xkwtyunk.html


<!-- 参考信息 -->