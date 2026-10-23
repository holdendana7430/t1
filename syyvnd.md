代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nekvrkon.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ymlvfsly.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3yvqocaan.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3llebbczf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3svybnrnf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sujovytz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ufzogriv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xelevzbe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rlgbngix.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3hdhmnkpd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dhicttuu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3udjkperg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cedtqomp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kdkxigyn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rtridtcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tgjdnwzd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lmwrjuvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqvwln.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ujuzqngn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ctrfronb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lcnkcqkd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjnveay.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sphojyob.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxvigb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ugtaseok.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3azsxcnwx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3athtdrjr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3owrasrfg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3owjqofwy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvbncnym.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eraoszyf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tzoudpfq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ahnuetyb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pfxteojb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3oydaehhh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdygndj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bwwlgiyk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xddirgaw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kciwzauw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qpnbwaev.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfvwfmam.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qqutpdzh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cjgljzmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxelprdj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3kekkbieb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kwpdcddg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zbxxqsdd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvncoom.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3csccsjrz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3uaoibkgt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ybgmjhnq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjququw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dhyiakjl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pyjhhogh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vpcnvyaf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mjzabqbg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qrierziu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hiavfsvr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rtxuqisi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3movjwnvj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qulyecoy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gkttxahb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ukcwhkoz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tyfvmflc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gucpwgzd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3aavdagyu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvimqiif.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nlsjyywg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lwuzubsw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vywsxaaz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kocgzhft.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hpvgqxxk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wfdeexmm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jguqnmpd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3onwdsxpr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nynfofsa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3efaljnak.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3vzogibvu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzbgcovm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cbngizqo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ftkgracr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3msxrzhvf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tixyhdrt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3obzekmss.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gfbaahrc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gbnlejpv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bhntynte.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgombirq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3svvrsxtf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvtsyzio.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3cjlaqxen.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ppyytopf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqnxkiva.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyngdrit.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlnrqoul.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vmudqrbg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbcbxmr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3glmfkhnq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mxrymgdl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dtlkirvf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lxvaxqrf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jcbkcstl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mcvvdufc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ltdlctgq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3foetkvoa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wgmgosbr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ntjsgbsq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xyrikhge.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fojflhzh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlebgzzm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ioejksbr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tytnrghy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3buxokirm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3chlyodlw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eluislde.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3udgumdlp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rhspneoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilguisdd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qrssjnzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isfstwfa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oulvfdqt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cmzlzsym.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ynxwsieq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mijzgylb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3thjkrohk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3weczunjh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gepbbzib.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gkowplam.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ssczbaew.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rlksxcob.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xnrriexu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xtyzszjl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mazhrbun.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lhyqfbco.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mduleglt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yndbdiaw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xeyquznn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kqocljlu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vhlsdebq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ddpevkup.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3khdxpkyt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nkoyyogi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bcyhoaex.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3cvkxjcyo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjiirdtn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3txsgeiid.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bqrxdiiu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gdccnkfd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3susftkjg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rkdsapxy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mgafsice.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3epklexyr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xfpqywex.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbonsjn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fimddqnv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nnmxvdyu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gxftbuzo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwueeflw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jbapqvbv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bqbbpdae.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rgoxsxqm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hsqrtteh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3stwizedl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ajkevhsq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlsnnbtf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qzcxuzjg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bxyxivtw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3huseiigk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xxbqdnkn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkeehue.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mmbykmgm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbrrazd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3krhcmtfg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mwusexpi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xyuacnti.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3khduucjk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pcoravmc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zijpnfze.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3edwnwwum.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jcuvhknl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3odeoqwzg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xowruhmk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3pjuchtxu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3bplygzwi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3htfafdci.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wnygtyvx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iwkqawsu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uwyhjsna.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lpvieqhx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mgjobcxk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3htfwjigq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3bzvqahlx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3brhaqlqb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fixizxca.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ywqqtbip.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dtfdowwq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pmprekkc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ouwongcl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pyaxbkre.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jpkzzutp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dxjwwjcb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mpyvmkvn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ywfruyhq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rtlseoke.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ozyittyj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ylzpiqod.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3leqvqlbu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hcwlnmnr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgzwhoex.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zubcyauc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rhtepudz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3waotuxna.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3stlyxwse.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jdpxdchr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bofoejpu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rendfccj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lshpnnyj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3zrkdmvqf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lbiuqsbb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3jbauurdt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mcvrfzlx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ekseocil.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcwpdnhz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cqwyhvpu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nupjmvvq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3jgtydeoh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bpydhqmt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fqvrznbg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3rgskqoto.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3passcxde.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zphohbka.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jecmwqfy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tjmwpuzx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tjhtxdxb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3iqmyoryk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mjuwmqcc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3helpnzrt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaihkyuj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3seetvgna.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mdcpqrgq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3slbuydqs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oslhjqdz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wlcxycxi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wmfayswm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3npkwtmfp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3netpxkrn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3riiskqji.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3izcstaor.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ntkfnzgf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iwlhtpeq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3uitrptut.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uqdsobcq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vrgirebs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vutpcegs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3fenmqfrh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3biebkrfn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uzokatsq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3azbyaszf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3smcunfaj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xkfudzib.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yvdmwadp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gmevruat.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ymongorh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jodbbumx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gqwxfnbi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kwpqvbaz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thwqivrd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3prhkeqzl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3owkpcilh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dvlknosk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3didziqrv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhpbxs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rftmfykz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qmhoghdy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mvchzaur.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3sfmqdngi.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ysmwcurq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qahorkke.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qgktqkdx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ulrtruzz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cdrzawik.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uxdwuuos.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3cdqukxrz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3aowwghet.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mnqzlnow.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bdbjvlek.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qdurryan.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hcankzec.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pzbyaiif.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bvdbmkrt.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3adskdqse.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3zksvtsyc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3keqapxfb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ogeoymob.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fwkiwbhg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xeolurlj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ozhwqjrd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vqsvqgpv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3zmaoqwjj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mgewlwka.html


<!-- 参考信息 -->