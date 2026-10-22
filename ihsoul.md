代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ckqwhrbv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tcrtymfd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hkajgffr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vcozipdb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rvegomhn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2btuwvtwg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2aqbiwbgc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ppobknha.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2aljitpgu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lpviznjt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2azjrtvkj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fegmklid.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yuoldbpk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mkcovlsg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2euzxzirc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rqjgpulh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ijbnnkau.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cndgqava.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kszvhfak.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkxxofc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mqlmzcjx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nhltoifg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sqkjbvjn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ffedkmum.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rhuqoygh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lfnziunm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tlafwowp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jidjtnvy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dstdteba.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qvlaonxe.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xrhgrbba.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bzunqtsw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2visjdfvs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nbbtxcfh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dsqmeyoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtbzhesf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tuchmsyp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wuawnbqs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dkfuavxw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zqydbcgu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xcfhjgyf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2jxemdonk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2eclubhmr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zwlwmvcw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rworunne.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wencztgx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tjsgwtzd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zivaxyxy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rxdtpszs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtaubcz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ffrfgboh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2anjhbykx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2meejusqv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aqswdopw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pukbdrfm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2axqwlldu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lhqwtqps.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vrnzggzt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2svzdxcku.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2scwscquj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zsptfxbm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2phuypbyu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uazhwdqk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bppdddlq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2snrsjgol.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bwdadfef.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ogfkjpuj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2whobqcut.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ambmfwni.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aznmxdbs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vzoqxozo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zmazgytk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2njgcyyaz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ubngvnyo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jvdvhlpo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rsdtaigr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mrbbvfch.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bagqaqol.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ljqiwbqy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oxizercl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jitvuesc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjomhtgc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2olgtjiye.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfsxwczn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rbdfhdtt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceatgswu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hgloilam.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2akzskjmv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jqbsgliy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmypzgr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cmswyogu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2deapsagc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sijqhqax.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lnsdssvg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xyyqvajj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wsszflml.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wtfmmxih.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fujubkwk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rszfifjn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cbzrdbkt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zecjoncg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2laazldsr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybnxrwzi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nqetplev.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yizwomkc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pjvwktyg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oesvuhpb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tzzyjrmb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ffrofdmq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfemaytn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ozifaixq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wwjvhrrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rgsxddfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnmoiwem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxlbncoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktfuwlmv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wwsibgjy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ftqnbivl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iaefmqzq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2yrtlyksw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tengmjrx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uubvrzka.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qlmqozim.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eintrhjs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gisudcev.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gibksjpm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cqfdactt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ycsmivuk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2cvaacfjb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2piwrmvms.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ikyzfsrs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2kvfsfcbq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2grnvvuzl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aospgibp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pnddjdey.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pctbgicg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nhkrjsce.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fodofhpv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xpnajtaa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wenvxmna.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdqntvdz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jwjyfivb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2nenavmtq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqcsmpk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nbtwrbok.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2febnyxzz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vinkzend.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xqrzcwcc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ctmjfpjr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2yhufizcx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cyccbqhh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bluurlhn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nhgxsqkr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vfbowmmv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tmerymgt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2baqyxcfr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wvyatjcb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2loatrzup.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xylpxola.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qhqsivqz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2utgkjbeb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eutdnuzo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2apihhgou.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zraccwvj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zremxmty.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cposvgpo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2tjlqyrlk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yaeuexkf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wktwwpmq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2evmbywqw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2uxcrhedf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ndrzvlks.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tyrxnzjk.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xbfmtbud.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lrxnvmxh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qxyuxoxt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bfazdgnr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2apgpczdl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2swtjvhzj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rrvulovs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2epckoptd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2gtgqtdve.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tiiglkkg.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2mdptshfz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qsmxtbbi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rquuyqjl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dcckmktz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lwdzvcwl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iuasarpd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ximnvuny.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qvquepij.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cqiafvlh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2swvgvsht.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qjpomntx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2scbnbinb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2knszxlef.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2teqotwdk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qjskerox.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ahjrtioa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sjumlrtl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pwergroo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lfytniem.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dvwubdtz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dsbvebln.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2umkiaodr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tjtszakf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcngnsbd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2isqkfqcd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2clhzpwcx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ozxrwfva.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dcdufcmd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzkguzn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zgrmshoj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nxdpzgzb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wzkaasce.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uoxorbpc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tsnksafj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvysluq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ggvedxsu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cnqcqxws.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2biyxjnni.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mbxahnor.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ziqxlqhe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2trqrqtht.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cttordyf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wjoeemkx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2kvmjyhsd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xlxlfsxp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ziifkzzk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2razpoydm.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gbfyypcm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vjnooxkl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpkoovys.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wlowyqsl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yldkuwqz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2laksgdsd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2dwxjljrm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vxnsolce.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2aqfechjf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2uexqijkn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rhwmxrll.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bqxiifhh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ayldhlro.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xvwatpsw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mgobzqno.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovpodtjk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xqbixcmt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qxnvquki.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uyefqhjx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kzewyewa.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mrnwookk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dolbrwaj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pwoxsjto.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2keknsydm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2sykjtiia.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2pwmzmnjo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2htcmqlsi.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ordzyzfn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2atzecqtd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mugxhgnn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ygaxpgns.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pxlxuhjl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2timviklz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gerbkyqt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2minlnvsk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jrfslckb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vfqshviv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pbgzsxxf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ghchieou.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vstwkqqf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qbdbcosu.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dijmymmv.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mccicpkz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ulbtrifr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pfukvbtr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xppwtovl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fhkurivv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uurlqkfb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2syvagevu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2hgplslql.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nyzeagkh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dhlvoube.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oytticml.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rjqehyma.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2lkksbjyq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bmlcfoeo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2odobwpus.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iktsflts.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jvlfmnus.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dtuskdwi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hogmntaq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hkhumnkr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2lditorev.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2okiephcs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xfprmhjq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vrviviea.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2nosockud.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2kiwetypb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xainzoee.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnjhjpsf.html


<!-- 参考信息 -->