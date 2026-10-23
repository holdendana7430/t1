代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wvnvunfu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ueaswydx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ctbbzkxb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3srnvbkdw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tnmxjvub.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3efofwzhd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eveoafpm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lfhshtmq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3heghpvoj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pjfvcxce.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cnzzrfej.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pvvmeynp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gssakcsi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yplvgtzw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3skgjryzr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qvglpkao.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3euvpurqc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dmeqauke.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3khwtggkd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nyntwniz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mibfzzal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qaglqfxi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wzasfrrp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3epyiqeim.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3soupnacr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hnofxcsf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3todecfex.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvjjkf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dwkslnis.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3mckaoykc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3stjtznnt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bhdzjxjh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lnxuacad.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hxdpwfsl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wqjnzniz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ydgjkqpz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zwckqajk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zssxnnhu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hoafubec.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kasdizgp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wuhsdrzi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3huzzrlsr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jetpdtit.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pnblgmux.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3voxvjlsj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3kvkyqcfx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yhspzofo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enpkijzl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qnylcucz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ypthalkd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hulmpxmo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ipuesfrn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjzieorp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qrvlqwss.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkjvusis.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hxhibqhl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlyhbi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kfmlpxog.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ypqzlahg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3orvlhvdi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3exhsnhtu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pcbsimzm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3voormjsq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bdkupofw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3shbbztpr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ndrhmjyf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zvmnqfkv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hswxhayd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jkigfcmz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iimyrfgw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gkzifzka.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jwushkvf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sacmbxod.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3godjwnqm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uathocma.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tshuopvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pporvjua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbzotdmz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uoydmsxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ealrejnx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qzqyhsem.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uiultxsc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ouovphvb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cioswnfg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yngmzvbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jnqyyucx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3onsxpjpc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3msdbbdlh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3outazujh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tuqwbciv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yjmmhvpp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vulkmeyu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qcrfwqea.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qsbbxgmx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dqnedbmc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ugvznbnq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dndtvtio.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3iapfktob.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vgitkryo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bqwfgouv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lwfcwsbi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjwcldx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fdmrdgqq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ebcvervo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3odoufncn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bnlvlybf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nllvlbaj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fefenewc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qlsywyyj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3detsoctu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3mcuabxgo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ulktbaaz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3esygwnbk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3czvurunz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3whgkniby.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vbatsqbz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jfzwialf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkufxcj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bijcqyxg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hdwbiuce.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fngakpvc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uttzbgik.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3hpszlppc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jyhbgynm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrptwxhw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kdeaabmm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ejrkgbdg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3khbuvyvv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3urvaqrxa.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfjqyjw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3eailxmsd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pdubxdsc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3geqtmmgf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kegnekmg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gfdfnzwy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3nbkdxvqo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3hohdqhfl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rahpsnhv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3facnmxdg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ysufufts.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3tsmrrjax.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gwtongla.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cwprnjub.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ufexttfm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3arwomsuc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3svqyxmql.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tatthabs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ieivynci.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qbtjcdms.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yqefgrue.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3olrpfxpu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fecriutu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3agmojdbl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wzwcxbfv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fxpuhkyq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3anthpsth.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xhltzmwu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3covvmacb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vozcgepj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hlwooqjl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fkzknoyo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uvdxtzts.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3clgogcxq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fxytutsf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uwbtxxtr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3siublzuq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nirdbubx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ajccwsdw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jpyrljxu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fbsujauu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xuojkuin.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3clopaptg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3feoybouy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3slsxkcai.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wtyhimuo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3cjrhwkun.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xwdtptwn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jwzseotv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pfvinzvj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nonndfbh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bebppwfg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nrafkjcj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3adrnwcol.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3valqbkht.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3qndbvyua.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iuevkvuv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hwgesnxs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wblbvpey.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pgnxbesc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3znddpzzd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ujrcxwhn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkqjxwf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3beezwhgk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bsnrliii.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gxfpiwhw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xnqqynkn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ujxrgcif.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eikhwumx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3grjkwxjr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dkvkzxop.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3owvekmyy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qduojkhw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3puvirdbr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mdcjimsh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pcbbwvgl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uhqhcreq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3qkjdlrse.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3frggpaql.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zulfiauj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qtnepmhp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dvcmltpc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3foanyjxb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ljoekltn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lpkuntun.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gbxyiaim.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rtewfovj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3pzsvrwwh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fdrfxaag.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nteaikoq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3aqgomain.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3prajdmnt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wkhtkclj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ncuvbmyz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3oluoisit.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3plshcuge.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3jpexvnli.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikiwmgdf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ymwwwkgn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3oovxbqnl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hakdtqbp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bmauyhzn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3azshderc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qpziucwy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3trruazgm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3neijvjns.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3orbsrcrn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dwlbsyvw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gyenpfbu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vwycerzu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zknsoxsr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mephlxzl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gknuqefg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rqvksfbg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3antmsrzu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bghcrgzt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qlwctsta.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eurndaux.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kkkjdmmi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3tvmmcsoz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3dubiqpsv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sylxkyhp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3goawqrut.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ncczlbxr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zlawpdgm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3suzyvfch.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3devfikjl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mjaulsxe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hukcotxw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hnodbgil.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbdhqddb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ikpnzzch.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3yyuseopc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cukqxbvr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bykgxdod.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fghcbtdo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3dffaryxj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dqhboqgg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uzrgcgfp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fmyzvkuw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pdmsduqh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dcsbtbsz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3takvzkew.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3edyhierx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iyoaaupr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iksxmjdf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3oawzjlrz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pxyhxsso.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dbxovlrq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3errmvwnu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gyrkvekd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lhowpron.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ribhibxn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pepymyuz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cshlctew.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3trubrgif.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fxckcwaq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lwddnwbs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3augibror.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xsycropy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cpqqvviv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xhbrzqri.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3afckdvbx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sgqgewul.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qfcchlhu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3osvyhzyh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pfrclsze.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3caamaklt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dymvcmjp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qyroigzs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vdwqrcvy.html


<!-- 参考信息 -->