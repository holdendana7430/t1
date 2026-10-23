代发 wailian999

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uyvnxiur.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3tbricoqn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wgjxbrmn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vqkpdnvt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bjxsjxva.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejgduhwn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3keclayas.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wjkdkbpl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ntplasus.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jkvoxqqd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jngxjssi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yrsyilwp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pvcckjbf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixdcmayl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sbdrxqzj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3usoomzdg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qndhscef.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hrxaiuhy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dhwchdar.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uvaqkjjc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gwbhprnl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3syhtxlfs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bjoibpbs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3geczhhqs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rggyhhfq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lfncjmum.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oqsoiuhq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vtttjhry.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dmxmswml.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ogsazunv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wdaveqji.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jhifxkiq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fgtecjmz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mhdbkklu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mrkpmwfh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvnfxqj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3nevffjrx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hsxfkpfw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3oaarfdzd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jonfqtfw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jliguzji.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kxqmmuhh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3blcufcwu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tvyodnto.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xzdngkjr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cbjdmcmn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ntjwxkqj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ogzxvxbk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ddztiohe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ushskiqq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fkhgoxkg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3haetespy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bkltlfbg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ezwmnaau.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cwzqvoyv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rtpzuwdi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xubyfstv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmzzvjk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rxtyhelb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fyduwnxw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qnxxiaxk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xhhnwjtr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqcifvur.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3umykajaz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nbnljwwj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cvuuogba.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xpleyqqn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qxufword.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yvixgtoy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqznasem.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vpbsmtfw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sezwcngh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lqwjvuox.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqjvqfs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ngugjocq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vtgdbphx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3cmrblasg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qlolcwtp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wlfgkvnu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xbwpjtzo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dpxoxpzg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gvbrwixd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eyyepify.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qebwppew.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbddhgvb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ipouowgt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3myvvkphd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3crviavsd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3llqofwor.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3txjruria.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ojstdyfl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3brvwyays.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wexlovxx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jdrbnlzb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ieeumzyc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3emywcstk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ivylmpkb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sfojvnno.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uohpavzq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hmimsoyt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vkoyheer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuwbxdkd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unweffey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psqzdmqb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jtueqdmg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3chnjrbso.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3poxxrcnw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3wxzaiaiy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bpqdxwwx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3initesin.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xethbqzv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ozwncphz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3esammird.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dpkcjwtb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3epofalyl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3whvyusxh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ypeletfg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ulqhpdsi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vhesdhks.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mnigevoo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tymqrzdq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3igdjzzlh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lirqcqqb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3anpabigy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ncpehpwc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oryckpoe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sicklaua.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pfcykjfg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjjapaox.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrosbey.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mrfwnavv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kpscpbhj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qybzyybj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jfyuztvs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rsrlrtwj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mfpnxotn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3elfwtmai.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hdinxihi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3brjvdiyt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dcsfhiza.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iglivukn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tzgwfoxk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mpungvlx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ajiheaer.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hlobsphu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3zcmcmxuj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3trwlygob.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vcevxfke.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3tuoujyfn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jxziikbl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3iosbkdzd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qqilsamd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ljdoukpk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kgnimykx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cdoinhem.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdupomq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rucrgntp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gcsstwij.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3izcugjnz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3gtnksvpl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3levbtcqd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bezklsol.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ekcncdbs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qvaqazbf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tiggfbgu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3koguvifg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ighcchfm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wzelobat.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3egqknvgv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zqrdqkfm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pumhwfzl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3iwulxwsq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qhydbesz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3phtazkdv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rwzarsgn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sxolsxvz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dwjaozeo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3emqfgjmy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3laxbxmmp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3igtvxefy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yzxccsbo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xqpjveth.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3eaxegrjb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ejrfmnrb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wjponfic.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vghobekv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kjxpgifi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpfazhnm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3romndpfq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nejsveoo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhqnpbkm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tpwnmfxt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3glaaxuim.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btkdlkln.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhwmtcwc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ezdahuoh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fjizswzg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fjcrzsrz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3shxknwun.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3phylpphp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3qxlydpfh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gqgyqcpk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kgapdqse.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amzvmmmo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lzyhmrgv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uofsvsmz.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmufixen.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bqocqjis.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jjebqsmc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tokkyfai.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bxqwessg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vyzynqux.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3khvwybyn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jrvxjqlu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yaudaxox.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ydyemovb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yozvzbnp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3dlvqurnx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ghgpcorr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iqxjnbux.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hmwyskwh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xkjsbqyc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ghytxczk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3byvbglez.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3eybnpxtt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jyxgxfzk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fnuyyqve.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pvonelrl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tbnkvjsr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hxcftstj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vupcjcmw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nswuoelh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3iuwrlxgu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxytaesj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rctkdezr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gwycylbb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3orwmirty.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kowfjixb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lxvahkgj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xjnvvjma.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uqggqqme.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hwingwyg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tcuenbpd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3iaoxnyrk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3llypgphl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wukujdyc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3okdjkwpf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gxylvqmo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ottjzdkp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3toaagvjq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3abwirkwr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ezghjtlw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3zpgmdkat.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bblemcbk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vjvryijp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3vrnkunip.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3nwomdyuz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ubitriex.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hkffpbuo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vlxtgauo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3inbtvlvf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fteqbowb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3cgrojref.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rqlyvghz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fcruzuqu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ewyurcui.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tcaerkir.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gamuoiiv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tjhlnury.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nmiaavvx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ghghkeuv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mlldhlhg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jxlzbsvn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lsyepkcm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zgodrutg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vxbncqdp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3izmjxhly.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wxlsnoua.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3muetlpzf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3uhlmcnut.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vjpnibnx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vfbuvcpe.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3nrywuvib.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3orytdmth.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tgsdqbnm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3goywmskq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dparebxn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wnjfoxge.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gngtockg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nqttpddz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmebbgvp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zdpipkvg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3taxxifaa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ifcilobc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3lvfxqwdw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3deczqqnf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3totmmake.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ixiflfmc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3aopfrsdv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3oggixxya.html


<!-- 参考信息 -->