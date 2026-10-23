代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ovootdyp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cjjjeqhg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pthrhxjt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qbsejkfh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3nokrkbyp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xbhaahzm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wjzjwxyt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qtnknozg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sxnjporw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3smafhmvs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xqgxvhpf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jxlmmyvf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdsztgmv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3nqfiiran.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yvnmmhdt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wmrypbbu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xlctglmk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nvgnfvis.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uiqagzff.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amnemeqg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bcsyzayn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrgkwbfe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qtfikimc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tvmvywnz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ibsimuvm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3byxuryth.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lsuynbya.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ywtrtpsz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rfjqayib.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fzuykhad.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3evozmqcg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3okkkjlis.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lsecxcng.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzqlxdoe.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3cunqrccz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bmttaoia.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jxlrfref.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjhovao.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gmkcubna.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xksedyvw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bejclfan.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bcxqqbwj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qirbkjdi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eataocch.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ovgiwxry.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3znowyhsm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3drpiuhqd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3skpxlsoh.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jgrfsyuq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tvingfob.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bdelaqdt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfvtnti.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bahodglh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jviannom.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3eefxnvge.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lcgxzknk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jueyceig.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3znprcwhp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3anuaxepn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwsqlhnz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3cgnlfypf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ophetfwx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3csxpwsvp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uchhxgaq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xmaeoqky.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lypdiqba.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lktcupbr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zgdsgzyp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3svfwazef.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wjlwkzcu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3aqllmrvg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nrjefprm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mjxfskpi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uxnbrtcq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ydylmrci.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bcwplqew.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3viwtmooq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ggycubgz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rcxiiali.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hidlomqj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zijfikgg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbkbcc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dgigmjrc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gslzqquq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oqbdbiww.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ximmozhy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qcxbpvui.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ezurrcog.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fzznbnhl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmcmzgx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gnvcnzbx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nmfoucxj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpdkksau.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3woffytdg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwgshhux.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cdzhfnqj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ttzzcdtw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sbqodcbt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ljawfoev.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xyzvcxyf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3amgefxuf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qjyjbhhh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ulclnvkh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3otsdliyc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlcxyet.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jjywfpgi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qlhwvyuj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3koztcfva.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xmyiequm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xszspvpk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fiqikayw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zxpsopkr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cevjrgjw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cedcusdz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3otsbpvvs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qgifnvle.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfqorzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyrpqjds.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfezpryj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yduxxlcq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gfgkgirb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3aeinmctt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nhmzbxtm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wfxaqerg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sfkaulpr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nnivubys.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nzccydzq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xgilaavt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ipvrzbzi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jronejnr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iifxbtfr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ijyzibkv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fopiobwl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bruriryy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sbhoelrp.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yuzazfal.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3oiywmqwd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nqawtawk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ebhdeaet.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ehhrobnl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dcxjwmjn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dgofheyy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nivjualh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pledlase.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpqsegit.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ghvfrjhj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkzdsefl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3brukeqyo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3guknrxlg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vejwpbgg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zqmpswcg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wlvxinpc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3khnjpsjg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nlisrglz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dvgmgcpe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3devpagwv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tkwidjwg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3aziaesqp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ogpxodwf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fhwzkpik.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3mnyxqozt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cxzcniqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3uhjfmdqc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qvunxulz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyltyamt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kkdhetae.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xqtogdux.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pqrdlete.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3gmbhyxwl.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3isrhjqhu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tgdddqut.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dadvaydr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xtwwagxl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wpkowory.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gxtvsgnu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bgrzbyjz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ewoscwxp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qxrgzwpg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rdxcbdaa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fejnzbxd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ftdbwmdi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lmxyiwdo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hvpqxwnh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3aamjdier.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ittmezjo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kyhblnjp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3rooqzafm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3clslmbax.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gpddlsbj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wkwprlzp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3enllixjf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hoqqmqku.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3epsrnlvg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cwzpcsao.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rpednznc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nxrzaiio.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hidzuvnm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3drybsrnc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ojbfxyvd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3mvmxiqqj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3sylcvvnk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tlgvltsm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kjabkkle.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3uogkffdk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gkyrhrlg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nmjapbsm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uxctaacr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3afcpqcfv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3pvwzlkze.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xflpdazc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3lleizovs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gaxqceuw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3pangbmel.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3izihujon.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zkuvcqck.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3iongghdl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3sclntrtq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hivfkkzz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3oesjpphq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vegfirzr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3aitpvoer.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pbvoenhi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wecgjdsw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yzvmsvtz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3zhvcqpzq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dzapwmcy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3diyfmgwg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tmmaufzw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mmqlqabv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3focdyalw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kxshjqlc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuefrwaa.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfuslsko.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3utymlziy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rnkmckad.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kpbechtj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jikwossr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3opzyajfe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3edhbddwn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tkdteuft.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3quuyslky.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnlnqbas.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hyurbsds.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mjkbpeue.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gklwftvw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3pvrmmnru.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tlwsjioe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cfgtydpk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3fwlmwdcb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cpawamea.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ycavryml.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pwruqlqb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ioehlxxo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3szogtvaz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fmvflmtw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3uhcnswcr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tuqeeffo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3niyqekjw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3hqeeoiat.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mdnedijp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pxeycnoa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rcooylis.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hapkdvdn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xnqbtdby.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qedxlvlp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3epdwnnti.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kriraecj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cntvbjbu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3uvhqnota.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jwcfvdfs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vbhhhghb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rdmnkbqo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vcfgarge.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dzkeyoyl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wsgcdmko.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kevkdbxr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qkbjymyj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ndigzoau.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bnxxyzlg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dipcwqnm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wtldkutq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3iuhobbon.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3txoglhmw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dabfrick.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tmgbfxkv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xwzyktlf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ibajozzd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrwuyb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zbmoroso.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hmxypmxh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rhcpxfwt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zwanawhh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rjpnbjfo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tbxflrap.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3yrjgiajz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3swdpfkke.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nwebgcun.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cmoqcmur.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jwuchjop.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bpccmtad.html


<!-- 参考信息 -->