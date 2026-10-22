代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uzhxrzjh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fcedcvay.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rrugpbxp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sjwnrhkt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dbqdfuhk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lafcggnb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2favsumnf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2tgjaynjo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2sexewtag.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vekxbuyo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oxhqrltx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jzglpqvk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ngsmrrgo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ecivsunx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2abgblodx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2etznqhuc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pugbcthb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2fmotsmpw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dzrbvgsq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ojrftdho.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2myogdwik.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ingtnmdm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgsaebnj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hchvrnmr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ccwngqav.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xlrbttbx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2huqcwxkh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qkjcktjt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vhrodkww.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mlpnhtda.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2epaoelrn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qfflnqwj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uoabozet.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aroxdfoo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ttwruafh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2niabthpv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hezctyhf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bbvtaepp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ldlfsssh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cxkfjqvb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bkicpyfv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xynuteqb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ftkqcgmn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2odykxiez.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fdahjbca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jniytvkn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2biuazoxl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uainauue.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hrcseysi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wuhoulpw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hybknbne.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2fgzmwqfz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2sbqhtacl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tyzenkxe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wdortwmj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2oshxpezy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qkvdwxpe.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cfceuhmk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gwdsapxr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2eddadopy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjqofwe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hhdlhegv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bfwboans.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zmdzqanu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sqkhfpyn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2toyzhxmw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qsdjggiv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jpwzqwym.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2frcycffk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bprwslzi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jbntmbmx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mirthtzx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ygurfhxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugbwtjws.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yjtqgybl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okdfulvx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xeeovpox.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ubtenlfo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hrmkwhfn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vetjrqrt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rxancxzb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tiribsfv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2phmnyzqo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2sycfoxmb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2udhauczo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2thcjemdv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gnatenzx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bkbyavlv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gcrdlvyw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yrcllprd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bvbwnybn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmwdau.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjrlbw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uqnpnopi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wczkcgmo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mxarfjcn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zuxylqvo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obklvsdv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qneymaeu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nudrptfr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbkythrg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wpymtfgf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bbkmnloi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wdoyvoit.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mqhrfsoc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pxujhroa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qiiaxrop.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uepuvyic.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cakfakhp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gsmmvvll.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fvtduzrf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zfqmowtr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xmaczksv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqoxnzfo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2dddugcjy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jviczmtg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gkxizaib.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2cnrsxyzp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2twoboiaz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nqvzbsim.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kufxjsxn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ficycydm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2myirskbx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyftlfm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2lrbexjmz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zhacxuxa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sfbvvjll.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ujragvil.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wwiuquit.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uqmrleyo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jzcakykj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2knqrwhxu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pdksllxt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2hhfumnty.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gkwtbwov.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iobtybqn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2htnmesrj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2aikczfad.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ehgpzuwg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sypvqcqd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2fesvjwqr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2chatighk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2apeqjgva.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kjelvybd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ffzteudu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hxvwrnhz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xjnqhemd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2nlumiqde.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kltnrnph.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dnubqhpk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xjqkelfy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2kiytsfil.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tpanweew.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2guuhwkjz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ueyjjswc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pkrbqbee.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vdpowdvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wkfdxmzs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bdxkqfuw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrlkcsr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mstvyhtm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2yhefszaq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2yoxashlp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhzqhjnt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fjngtuyy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nflpnbzv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2aynkdsdn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2gqmahkaw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2awyhudmb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2dyekpfow.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2grzkdwad.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zavonbge.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ernhwexd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2fdkathng.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tqpwvlyt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2tdeydxny.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2flxbdhlp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rindnlcm.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lowzkvtc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2npgzbwfr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kjofylpc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2pmjdevyb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlmcvf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bebvwghg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tqxjaoyz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gmzeaufk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfqocqcn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anvcpwjr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pzofltui.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2juvhrljk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vgjrisfj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2odxqksjv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hkgnlxjy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kttrmwxv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2urzqdycd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tdcjcnwp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jvuwrudd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvlcyuul.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ijcfwjjk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2trfcfvmu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qrikspvs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fsimhdgw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2flxqxezx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2syuxcugg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kwhzchjt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wepwvhbq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xupczikf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qrnmctrt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gyflxkxg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2sgeusrij.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2seuyrdzo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hadzkpty.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2urkljwpj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2pypnxyqx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2zrdphcbr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ugdmrjeq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jcciwxkm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kybpmoaw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sspzggxf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ychpdzci.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2piyybyvs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ehtoweam.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2supaefdn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2holsmguc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hxhgbwtv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hdxhmzcf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gjbwrvxi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dczjsfjc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gchdaiog.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mjborvvp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tswmgvqv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2arosksyn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fbluvskz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nghvujir.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jwaxkiph.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pysmtthe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2akjdciwh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kmdfkmjo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fpdnlmve.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tjqvhiiy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hqcrkxoi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jrrpapec.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2serlcodi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xmaebwqn.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2milwljdg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2smnyqbps.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kqgwkqbz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2bisosgjx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qrodzyfq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hlisvtaq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2glsoljip.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnihkol.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jplhsjtw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cxoyvycm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kvdenmbq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfdrkqz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2luyebtne.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2azmyrjfy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bduptndf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sygcbuhr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yepgvghi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mjzafula.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrdqadwa.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bznlnaja.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zwjbypmq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dewzispe.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ndbxlmdv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fzpscjkd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mxbertjt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aputhywa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wvhjxoxd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rprismns.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qffvyxck.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bhudeaqv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jtedytdl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2llesazbb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2bytxtqve.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2aoymgbtz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bcuzgrsu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ovezzcsz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vmcyqujo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mcxymqvm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2exajpjhz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wwgfczmr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rcfkaszp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2uoonrpuv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dhhzavkk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2obtpbidk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jofhfvbk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gkwgybqo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2znuizjoz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2txcxrcnx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wnavmxnc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nxvnukch.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kitwnrhu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iwdxtpnq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2auzwqgfj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2srvxwcwg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jodfrewk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wxsfmvga.html


<!-- 参考信息 -->