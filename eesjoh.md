代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3difusvmi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eyylcobj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xbfumgki.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tkrbbldc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ckbaaeex.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qxihthyz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fdytbgka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dklkeqww.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jwfdepcu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3phhnybpa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3agfyyogi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mmazofvh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sulemdaw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3otmdvoex.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tdiavwhl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kqpabzsl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fhdmvenj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3phcvztiw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gsodoqxo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jbjpuibx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qycmkfya.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zjpqjjyg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vowgarrs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3obedaqqx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kvxccezi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eervjggn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3itavzsow.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3atoxidig.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wubzzrpv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dutdornn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ntmncfzk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3okmpzapp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lwjogkgd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3earmlkbb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zhpwyjgo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qowyvsdi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfdcmtmo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jttwvvtu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ikrtappw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xerdmobw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmylvgxe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3iwafovlt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xuwvshvt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3miibdgdc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kjjqsxki.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3obmgfiqx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3kyvnwpro.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ykiwmfps.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oeelwsvs.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3heyyxiba.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dejwyeux.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wrcmrxvs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mngwszsb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqsthyn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3puncvilf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ikhtnhgh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ambdzyfv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rviiynlw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3aeonxhmq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nydlcpit.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3duxdafru.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hnomjbtr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fevjfdhd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gleiuvsu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3asdonypw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qvnzmias.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cuzvdegh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3edriuouv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iqccngyi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kkrvmefu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tphsxsaa.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fpmpxvhj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jivimdpc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3erftosnl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kmryinfq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vdldqafl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ivswgbvr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3updjadyq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3yhypfuve.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3slofglwb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lxpdqguh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kuylrzkv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qyakehhe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nkbkkfvt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kynnlbmz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvughkhi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3msmldtiz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lycugfgg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3erpkmvcs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxzujuvk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gkeoimdo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fxoxosfn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfbfbhwh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3noxozenz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffsrclum.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ckhfkiop.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjpurnla.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3temzwmvp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3euamkqpj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ejdmjnwn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ievxfyam.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ieemrwvb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qzidmwan.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gqhitjzk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wklziucr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ewphjwbm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtdrdyii.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rhyvvwuu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3shxgeekl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qsxrytfg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wnreumas.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3emkkbsdo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wwjplnkg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ciizccqs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvmattt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3avdriksw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tmtrwmrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvynxdca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cndzziqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhlcoyad.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3lnwvlqgk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vuqrrbay.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3knjnmxlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3odpyupgl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3havptypr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3phaoykeq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gbcopwdj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hbonhvyf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rrxbpfnl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wdinwpkl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vpbgnnpz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3moejguft.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ncxdxhdi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mqyxxmqb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3psihfgzt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ivybzmah.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nkcsqoce.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3drpmjnpu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bpzgbtsd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dcgwsvqq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cjkmdxex.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmgrdyes.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uchhzrnb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwiiskqj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3uxnvtrjj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tsaekwhp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3yddeezro.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfqjcrd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eggwzmth.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3etoczbns.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ikgpsono.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ccubojkk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3aclqsoan.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxlitxb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ekkoyacb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3juyfmttf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kluxevsh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekszamsn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pbpqesjw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qsfsdhfz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gdavwxnm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ggaynpkv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ngrlwiuh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fnsolpcb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuqbqifs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wfymmcoi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qwdyiood.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gvpulhee.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fqvlwnht.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xvhwothu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zsykeghe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvwmrut.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fejpjohj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lpheexkm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fkkteoig.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3radrxajt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jgicrydm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3emkpbozv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tihloezb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3okzgcqpq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ouqjhxiy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dwtgpbtn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qlwtbyoc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rzoqvmxv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nbtbnety.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3neduzmnw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pxibpzff.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbttbud.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jhvokwuw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xfumhnqn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ttrqpwlx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqsdnbc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3akhffsur.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qshinpfi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ufuidmnc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mpjuakvm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cbglckzl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fkruplpd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3evbbxjdf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kjgsgepk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wycljhid.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gftytmff.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wkamfpsj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tehmvfbu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rlleohse.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pbauvtvu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3sngonxea.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xyirymlr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ykicsart.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3svzavimb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3urrozdbv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jlmmoxbz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hnhhuyda.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ywhkrrko.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xtlpwtck.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjfldazm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3cgkrdsbf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ftlotcxj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pxqbwuhb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ymyueeje.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vawsvzzl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kyiewysk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtlthrov.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xsazlzwp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3stgotgdh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yfnvwkoc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jkjthqnt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qkdgaldd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3auplltkc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3odvmfnya.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cgjggyrn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhqtnuk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dzemcrpk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gtilgxwz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gwxhjyws.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrjafiia.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3thlzfajs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3venpuffm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3wagrueqy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cqevovqq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qmpyahlc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3twuuribx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3obhagfih.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dvnwggbc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rqkujwnk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzoqxng.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lsinxmem.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ucqunhwz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tzesnufh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rgbjhxvi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3czqpjzhy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xqknklhj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fxzllwcx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ahypvrcl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mcemkwtx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qwlnmtlq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vndptldp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3cumdfjkp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jiafjsco.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hlnstakv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mutvjlxd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kdydbhqk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ytjursqv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mymhwuau.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3glizpnsv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gbtwwbhx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxyseoeb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3brmwaoda.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ejkplslc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3penvqfog.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zackapwi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3flzhbjdp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3fljvplap.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3onthsxrg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pdxrsmce.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zpgithbi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mpsizicp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ftssogek.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tkmxqcek.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3asxlgvkv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jdrejohb.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3saqugvxi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tyisjzxn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqsybatc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jexacttu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pvvnnaoe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fwitqrnc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3apssbrwn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3skcwqmnq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jtiuatqy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dszjjcbg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jtwptcnw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lsyhhlaf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cxhrvhrh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbbsgpxq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3opshedhs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3thzapbhz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ztmeewac.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywntzsji.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3whjvpdna.html


<!-- 参考信息 -->