代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uvzpztqf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hkmjctvy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lojngdah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dqimngaz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vypukhmg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hsjnrpup.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3oawtdhuo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tjmffprl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gpitjfkh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3guzqkrsy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3djvvvsyo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbswkadd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aviubhkp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yqiazrjk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pxtmmdhm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eysnacoy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zkueadkw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jxevilsf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fjnjhuxj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3gftsulhd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sekxijpj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkncxqf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tnzzuzci.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ionqgtkf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zolfmrdf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fboltjhc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpgavfog.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kkdlzvzl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3cgaibmrz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3nnwghnsy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3axtxaqrr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fkbfbmvm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vlrtvrkt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nqxanrkj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hkliurde.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qrwblrbh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vvfjwaxb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3odahlaku.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3epacaaig.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zfhbzmti.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3evxgkajs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vqxlgusg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ghkzccax.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hyyuwxts.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uddfynii.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbipnedl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ljhgdrcs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fvuhvwof.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yifuxeki.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bwvadabo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dlqpbmvq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ljffydzx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ywgmkija.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3eambpciu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cusiwjei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3eutkjfwq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sjmclrhx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bdenqmon.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kphkrnvi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wwdhncmr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xccmnwrf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ifyktsnq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dvkxnxlw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rnjkykod.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3pqzpbjer.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yyvwchus.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wllwymiz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yzummlcy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dcybaugs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dzfxtebi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wandapxu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3yyioqegc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hoppxpbc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ihqzjrdu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fgkfqwwn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3whquqlxl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fcteyaga.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3czphokcy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yfysktso.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xjwewath.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fxycnfqc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3iselsqly.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rkautltk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqncpeko.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3merbnqyx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xjietriw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rzsankuy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmxcgph.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vhfmoctg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiwcpqpm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vjhisbtf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3actclkyi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gfbqhkii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3epdadvjw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3owkopuoi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qsjgeqjw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tzpxygbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hjmpzofj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3upynmilf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xlyaizph.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbngaczh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ycpoquvd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bdpxwnwk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cafsoyeu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lfoxxlxp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zvvylsmh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xuioyeku.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kmhhknug.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekkssjlq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fltauvrj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qupadbkl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tdiadlso.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yrkrnpxv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgiskt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kdzzbnah.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ujxnlxlz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ypigxtmy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nnkjjcrh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3evennuka.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rxomehol.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ovadfjgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezwfzhad.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ktzorlhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxgohytb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tebcusns.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wgpbowuk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pgbvwgex.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bkamabqz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xwydrytx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3udddnmhs.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3qzcmuyip.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hxnxjgcb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cbklheso.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yqyrpnuq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zqbykvzl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3vpoxfzgm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rlpwatjz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xjklmipf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pccrdlbb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uqyghpkn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ihpmczar.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uqpdeqaw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3msgvlvdy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ezvjntnj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gvcyxavr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gnijeomn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nfoairlo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ctfofvjz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vqnvkpnt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sratjems.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pehyypfk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzubjg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nqiotsqu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kyzjytat.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rwenhcqt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kpodysmo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lsseouim.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3umthoifp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fbgrhldu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lodepxny.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kzozxelo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vpudtvwm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ecdngort.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxjmrwr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xaxdqwhs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ubyeyhui.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3egidgmgp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rtjxrwet.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3pvxlkxqs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vnnpdeci.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3costqgiq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lpflbrlh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xidbauek.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3csfoujem.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3odlgcvmx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jgnbbbeo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rsbygebc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3thobswhd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3thjqepft.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jwjojstm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3knwihtgu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3iogtdwqe.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lngzqukc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yaxpvcgj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iumaydhp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jqzltddp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hlyimtpd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bssmxtyx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ruwakesa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3etreerja.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bqytkxpv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ivdlcyvp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3azchawfj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ylkmisem.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wcxojdnn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nuttsqks.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3fueprsrz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xilxdbmj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3uwkbzjlr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bkcycmao.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ztxlmadu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rqgtsluk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vacjnire.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3eelrezll.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jfdwnfac.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dyhpsuid.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wkqdpgtr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3eobdxngi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sbvukkjl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3otojlqjq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3twnopqmn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3coqsnlhq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hpimafsw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sybkwkqj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vsopgcxt.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hypieirk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xfpxaspi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3lqiwarpz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zobzsuiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjueig.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zunkptzw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3spkuhqfr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qlzitxpa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phmufkhs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wneparvv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mtjtlmkl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aolpqcte.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3muxrjzpu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3owhyfjix.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3oqfkanjt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dlrcvmem.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3edgnnzdf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3omjqnawm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fcqibhjv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yqkdlbnl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdqvtzro.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3loaxyjus.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkeykbxg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3onhceywp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3thldlemb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3cdaeujbu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvsikbpo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zpjxsuus.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjnvtgl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3cljupqid.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onmdmzkh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ugdqgyot.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3chwgmqty.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3agtnhlzr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hixziosj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kdnqwtvy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vuqyagjm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3wqyhqfzv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ogllfvvk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uyknnudk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dllyoxrn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rwiboctd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wtfozozd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yagklora.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3owwckziu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qnjcgfkv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3irtzrbuv.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3odxsmici.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3uodgbuek.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3opiyogdh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3peebdrcz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wlhqbhwb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wnvqrdrd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3seyprjtf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3uxxhrerr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3szvdivps.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ruixcyag.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3sbftstsz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3afhyisdg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3byjogmxs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3slpamsdo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3drojaldm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jxyexgbb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vwyvaplv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vbkvqufr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cvaknjfh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zeshdhkf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gtudwbfw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3pbjeufyx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kintdctp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lrufifgk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3twjoliqu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3oriljcoh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3jqnquaby.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yvrdzqic.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bbkrhzsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tgizgilq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3yykypere.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vdhgosdu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yxsdetqv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wogvdvvr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nfwyonzz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nizcueoi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zbrrrjqz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jqmiudog.html


<!-- 参考信息 -->