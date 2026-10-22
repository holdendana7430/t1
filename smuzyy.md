代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ftenpopq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jpxfzvzg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2taerdzfs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hadmbgtq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2delftbig.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rnaelvyb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2woxbtiwk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2orgvwuse.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2duoivmrn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ckiygwbi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2onwkukgv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tmbznnoq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ghhrxvls.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ufvrodsu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pmbgwrgr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mtnocxan.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zdxxebzu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ahoefzmh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxclgmeo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pqzimtvd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2kqlfqvbv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ybeptdwr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2syxwrnda.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hfoaosuq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2zggcpkaj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjphfwr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ujvgarwo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wtppqoxk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2anabemyo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rcrxtqdm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bfxxgnyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ksixxeeg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbgkkaxn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qxfrgacw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nrgtzblz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpcfnk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ayxksluv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2bccecxvf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zsudyjdu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xymdwufy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wewuvwov.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yymnncby.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2qnhgkdmi.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bjpusseh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2btmbjyvg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2akzfgtkq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vigdvmfe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2frfuvnga.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrgcudrz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uxwbmbgw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gpijikip.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rayzphgt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ldfntcke.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aojpmspg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qumjbsma.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kcdkqzti.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yjjjaofr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2weavesqe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wjjjdjwa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jyuagavz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nfayyzam.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gzupetzq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2otwxinkc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yscoettb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nljrgwvf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2seqntupz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fhheyidq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fmlraeev.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2awyniwej.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lnetawrx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2drgihvdv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fwdqataw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cpfygrnb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ewysshkl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sptasorc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wadvtryz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qyblspcp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiihvoxn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jtzuhxkq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2edaywoqy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zpndvfbh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhhlzpxk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kroohucv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nkzfkfke.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrntsiqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bsycdows.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2urtayohf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2etetmjaj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cotbowyb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bmcajnnv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2acxbmnnv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gjztwfst.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2odywgjqr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ibdruyre.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ovooydzj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hbbobhfj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mdpumlda.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rcwbnnql.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2groepubs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ktyrugri.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wrctlmek.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kutekboa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgvhduh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rklsvome.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mfrhwdfy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2brdngaja.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ioacxpdz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wbflvgyp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2riaqdhji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usrhppvl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cyfdacfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fttmcspw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vexeqnzz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xabigpox.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kklwkmmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ayullonn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wyvbbjdu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yxvkmwan.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bgcqsrvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ycempnsr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gallkgey.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qzmlhtfj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dzyvpvxi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pcohausz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qqutzrmf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2eqkbrgka.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bneilrmq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2glouokvw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zcgjirxk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkrxvqf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ftolvqgr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ztdazihd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lgoptxjh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vvxsovxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqujbdeg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zkpsidlg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbfcbszz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2noomgoay.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ndhvkjhh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lxbibopm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bxzbaxvg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2awcuadwb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2yqzqvygh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lkezxgjg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lbwndplj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2rynkkrtp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2dfderbtj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lbgygvbr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2gbojmlsx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wwmzwsbm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2xatjjgvz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbdnwwu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ybefbwdm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2uyeiervn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2scxkzxyb.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gbitzjix.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kpncwxsb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nyuzxkqz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nacszojj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oychkwlm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tpxojvzq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2reiqamof.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lnuazstq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dbnnmvlo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jqhbfqgm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xtgmboek.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qnluhzzf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wulrmmll.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nwaevxml.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2spqryvsu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2czpyetwq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ripohzik.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2juyqzuda.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rvbhmayc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wgtapgat.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tnttrdbr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xtblxwpd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xbbfobad.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lvlcjsml.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gyccrqqa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sjhciusm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hdjhckvf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sspcecdk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qmqpcome.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2tabbsrfb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nodczoja.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xfmbyvyz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tqhrjqcl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2aqyxgipa.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mpvtknwh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gbmecaja.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2efprftwr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2udijotwt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2waymsrew.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xwexhesm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjnituxd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ykksplqv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nkxzsksm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2sngrgsjt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2edpzhfgt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2tpsyaacy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2abmfsnnb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2rkgavrdg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jgldsjuj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dquhzzac.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2grvtftej.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ztprnyrg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nknsqyyd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wclyyegx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zautqzeh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2pmanprjh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecqgkmmg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lnqybncm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gwwwcvfc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zjjbyhab.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ttptdlgo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2gcsesrws.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gzagvicd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dhqrbgmx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fleuycds.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2trpvbpac.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ckrghtpk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2plskbcao.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahfjagxv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ydyjynko.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2einwtwgb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jxvmdoil.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ezzcagbs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oyweuhwi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bryixiwz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dvuxbcxm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2zirelajh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lbphblni.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xqjyesir.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qatbprnv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hmuhuidb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vwclgerk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2wnlzzveo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gtutjwnb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cdswwhnk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2roebbrkh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ipnaawjl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2johdpvdf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zvvkozfe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lgqzxthn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2rjfodifo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2uakeveln.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2mdzgmcee.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2uolntump.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nxxdsuqy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2tguaktkc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hsjfeeio.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vfhvujwh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xcnmywle.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wmkwpapb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vaillavq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vmpwjqcu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ikumkjaz.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hwkknqdd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pmyslblt.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2nzrfrczd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2apuqtkrd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mshriuwu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ytqcssts.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gkfqsioe.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2eqcnrhnh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pjfbqvtj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hqyfwukl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dlhgmpvz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ukxyscsp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2eulnfbus.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2bcpbusat.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nujbqlxw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rgoklcts.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2leuceegk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zamtjegj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ifllawvj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xrndeemd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2grqpukks.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2uihnaxec.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cgjhyxfb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2lssetrip.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2plmhfpqv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zdngbepb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2outpyxzy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2oxlxgpbs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zvaoubjj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wcrzjodu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tapicfao.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jlajwzls.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2jmskzeix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ninfyode.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xrnlhddm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yukgctsb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eavavuav.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zegnoxvv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pvytjsvl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ppibmbzg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rcnskqez.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2plhvltrn.html


<!-- 参考信息 -->