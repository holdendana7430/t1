代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zibnmfez.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wolwybdb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2idmuvnqd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bwjmcaws.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxjopysc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lablfuco.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2wcvzyqyq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tnjuqjqm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2igcdyugz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qwthnxdy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ubsbamxg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhwgwci.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bejgrqmz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2idcffapy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2keduzxqj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ehqkedwk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gvtwveao.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lnozkjxi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uwekmbzz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2efipmbdq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mqnyhnls.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mpcngwoi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mpunytqr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2buppskik.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2znjjyfqu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vrcdlkld.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2minsltxs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zhsqvxmf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2impluwwi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjbxoat.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zgswmcfv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tvkvbziq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dsmyeuiz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jtukeeos.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ipwaklyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dkhprpjs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2bypfzdsx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2onbvtsvq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qalemzvv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hzgipxot.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hpkfnwov.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vohwcrbt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fzpywsfc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ctglpgbe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tfnbjwfg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2villjyum.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cbestnqx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bmnoyscj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixcjyigf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lmoinlwm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2usgijmvj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoundfup.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2rwodwvib.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qbnncfak.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zssdsiga.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jcyqadhl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2iglgpxkl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghiqpsny.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hrmtktht.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gqwzlczt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nghtkccv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dsurggru.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tuyiuoyh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xmzfubjs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ydkoumbk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ytrqtnng.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2szsfibai.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kgbbyhvm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxcmlskf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bwdfjdsj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rblaskij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ahtzwffr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uamyukrf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lrbwyxwc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ipeywckx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2scoeyhmj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jzinryne.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pwygkdwu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zbkrhnhb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zctygzcr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2venyuslg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqtzccgy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qranfatr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pvanauja.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqnkximz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykgdjous.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wupfcloj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ekyhphit.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bkgfilip.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jvkktkkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yovujzml.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2htxchtua.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aifmvkys.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2juchcptn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yqklyzyz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kgpktjcj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2narqndfs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xczkvcqc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fbjtnzpo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kapzftzn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nlhwdshm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ggqfiagi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xxskdenh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tkqcnxad.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zhkpgkyv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hayzncis.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqmqvya.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jwsurtyq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yfnthuqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvatdglu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rdyvhuyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgxfbyuz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2iglnsxlk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rwoxhsps.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jfmmrenv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bkutfcea.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2brdadduj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bqantbre.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2igfflsml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cahbugpl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2htjtnlrx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2enfwmqfo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dwtxlhbs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fagknfcs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kdhmjvtp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2lqfnbsht.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ejjijjhn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yruqcmyc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ntqcqiry.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2sblicotq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jfccszce.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wwteubuy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nnngtwym.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqhcovx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2clwiaphb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2anieegia.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybotflig.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mvucwnhp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nosnfzqm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lydfeoxi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mcxypehd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qhsngnzt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pjgcomug.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2iwzltrcj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zuxlvwdf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bqohaeos.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bmrqtcmz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yctcfjsu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zkoccwtz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdefgej.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ldhzgfug.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2aklmnruc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jjaswfqx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tnzehefm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kebmedxk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2jokgkryw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dpohwsvm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ndgsohpx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jwquafeu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ftbmxgvt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ttldgqzg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mxqetlqm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2jsyaesza.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2flractpn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xpvuuilv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2museepml.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2lyybhcze.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wukzddgh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2scqnxkkh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2nhdwgayw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pxkzmudf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrlhnlp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ewfdrfcq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sjcvluqu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bspphmst.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yyqrhjbr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mvkjwwgq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2maomneku.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kkhwbzly.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rmzobyxa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hnpjiims.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2boxlqgvt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wmvtsucl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhntfjq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bzxkkxyp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rrgbsuce.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ckcflguj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2rhgtkylf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2vyouikiw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tibgsuar.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aafpdrcq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lmypnwje.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2msswzuno.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2icdtopuu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2kazdxpcw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2mpikpvcj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2oebovjtx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ntkubigl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfmafbaz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkamdvb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2yrvwbinn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsetahk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yrflnmes.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tnfwavdj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2qttaxfca.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rtxfwwau.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tverzouy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuhrjmnp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2trarfzch.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pctyfcrj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uzmwhval.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vudvtoaa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uhgygskx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mfkfxlpj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgffgztj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ardpqcxa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kpirvvhx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xzdquxma.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dymokavz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2rldfifbf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dzxvblec.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yriwzwlc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rycaxaff.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gszityqb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hsvyuoha.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zcjkszza.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gaukeazv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tiivxuym.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lkxgtirx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkfeosd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nkfnulef.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lbuaizde.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lbvdgudo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qcriozxx.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cmpdxdgw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ncoxkcgd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2wquudgsa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vxedtviw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2eceidvoi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tuwbmxgi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ecxtowqx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ypqnsgda.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cuuzgqwy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2baylzgsh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ppngnytq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ggcigxhp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2snjrecsu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2yhidqyre.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fczvfgay.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pugwlwwh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2abpghsbh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dtszlhcv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pffdujbq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sznpbzfa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cxeedzpv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xazwgwdt.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2yqshrxxq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ppzrqouy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dwmjtzmg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ranosqga.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2apgmqneh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2tganxttl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ozdnjwhm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2drwregps.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tsthedsi.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ieurasjb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hbbkqife.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2rmtzopbs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2alxnlfvo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zslcvsrf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mikhfgcz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lyudrfmw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xmqwbmwh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gkwpgykr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2owcvculw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ilxigqss.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2oviruvjn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kdxjpgnm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ildewwhp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ajedletb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2iupsvrvy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rmsfipby.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2dtgntcgt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hqjlwxqw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rsguilaz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2nxrpftvb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cxlbekkv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bsaelvuf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2yujzporf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yshrrthx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2dmuxejkc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2udvipszw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzqvttwv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ikgjxmzj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tahmqxoc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncicynmj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ucebjaju.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mgyqjefi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ecaqotcr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dcoqenno.html


<!-- 参考信息 -->