代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxwxdnkt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3daljvknu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mblzudxb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hltzlxlt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ieldtrws.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3quewyxid.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3efkjahqf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wkpxmzhj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gfcpwxou.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lubveikx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uksxcxib.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lfdwkvnn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3fwjxihok.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mpmbhcsc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dcedettu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dedeiztb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lfdndmjx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3evsgercb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nsskuudi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wfssapck.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujpdxmzl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uxpqmfjx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jlagnfeq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kufsmxjn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kkexghjt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3iemqglkc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uzsrgooi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hdiizxrr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3snnhifpl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3uoasahni.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihxyhjws.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3brmwmymc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tixnlpqc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ngikhira.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wfuduugz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tvojhddv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yyfoqwjz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ylpfbryd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gnahkqux.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3juegvgik.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yfiezrlw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gaygxxjj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xoedjrnn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3csgnaqxl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vkaggnkx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vibxgnlf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ihwvstvh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnobgsvl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nxdjipdi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qvwyndel.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yiassphk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sxwbmrkj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jkofqxqg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydtshpec.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3edufiltq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iqqtexix.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dumyybcs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ghddfedf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wtqrkseq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pecbhnqq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3awwjlxda.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oiruuawa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qghttifl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3khcndeok.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wayaooto.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fsiiqhqm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tpethenm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wjxevrsx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tphthbaz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3katlgsyv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dyxtmbgj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jpfekhtq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3epsdrtym.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eqsxipqc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3giplrlii.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tehxobaz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pkllmkxc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rvzroatp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zisyauje.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3irsppfmc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fkatrejx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izvqqzyz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sccycklh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdfjwsma.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3smwkrnsv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3clxuejco.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tirvayey.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bewujvzw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hrlbednl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rdkxebch.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rtcrkugb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zpmgkzcl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jqjxocvf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qbquakwe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dpcfncth.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pxwrhole.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ruasgufq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ejfnhfdi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fyynzbox.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wrxcvakg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cshvuckg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xahtbqhg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ilpjwckx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xrxnpull.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rpfdxjhh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wkomzbew.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vxlvtiov.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mfawzwuh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ieadtbmt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rnuwgmrq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3buifibap.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhkgael.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bxuuuvzr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bfxbflur.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xcwxpulv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tmdgbvhe.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pyfwndfz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jowxnfwe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nkkyvvlv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ibvihdkv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3szfsnvos.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3gzncmqmh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vbxtzefc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zckevvkx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ufavaajt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3opxsfqnh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bpzskoyi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sgmicroq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpljcesr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xflnzrvg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3giqhgazp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rimshsbf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jmskkrfq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nnrlmjfk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3smcqeywk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxgrdqs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nzhmdcbn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gwhdagmo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mtqrgywi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vgtberdd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3guuoalwy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3olnzynys.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hudebufn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lnfcqdvx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ukqalhjd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xdazjoos.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vetpvplf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3mwrfxexz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbzklt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fqopvjod.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ltlyyzuy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ywlzhahi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3grclfjwf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pjshdthj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3iclywqwv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ayxvwxms.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3crbkhqpm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3alckefol.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3pzwxjqvu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pcyblxmi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bpfxombz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mpivzwvw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zotmyyml.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bbjjkezd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hnajluse.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vzaodhnw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bdgilpib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3oegufmpk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fkfydzpn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3cwlwbopz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hlwurjbn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qqgnekcu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3icbhdyhm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpelimro.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tgasltes.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kjpyhmxc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3eiegxzhb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ujtweona.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ebwogjih.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvtscdck.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vaywiyjh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3chahbspx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wixkktzc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vqtunhbj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dcbczwxa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gjpkriev.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwoolroo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3npqwfxdh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3cimlhexk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aejfibia.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dtrwiycy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vaouvlwg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yiyazhmn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3scomqjgm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hezgrxxy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnptruis.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yquxppoz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3flhyywtl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tnphjvhh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgsiswtx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3glvaphjv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhgtglgt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mzyzxmeg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3erpzszow.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mvcgndwf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3oplzshwf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3jhdtndtl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3diplfjlf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3aizicrur.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3duvvcntb.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cfauzcdg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tyxwmtqv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3evwxtntv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pxuvguui.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ioihldsb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfsqjdey.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hcqsbzhs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jtjokvws.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qojoowkr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3grjjtyrd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3seuhjecb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hzrculld.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3onuvmvmy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3eeipmmxo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cotvyxqj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qfbucmap.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cmczzllv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qmnmmldk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3exbauabe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vhogasnx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hsseehva.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dnlnuyhv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cwwjdmuo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rwgsciiv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fdxbfoua.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jpunomet.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qfjswdlz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3njbhliul.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3soyplqjq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3svdapknh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3nxdevqzz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pqkeejxt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hqtflnqm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3phkehajs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nfjaijyi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3isbawbua.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mvubtium.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mdphilew.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ooqbdikp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgrnso.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qpggsexm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrasho.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zvvrexwf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qcljzafs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3khihyybk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rsgzcvzr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qgddzqwc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3kokpetpl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mranudqs.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3bretsbei.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ykxkircm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jrpoides.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rvknoxbu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yktqjzmi.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vvdfkgga.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zxrbmilx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mfkyrjvc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fytruayw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3esvpzmyg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ylcvjejr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xxnahizd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jmzscojk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mnobolgj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3uqaqrsfl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3viratlqt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdonytvy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3gqibfajv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jofrfgud.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lhreihxx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qsglzqbk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3prxzwswv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mkoqeopp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3utmsishz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3etkwigmo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3jueetppn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lrldznjq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mdcgejjt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3btofsokf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gtgvelau.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zfoppzch.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nmmoqxmj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zxmfqsdk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3muqwzixu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zuwupqjo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gromuubu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3seqgxblx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3teaisbcg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vytxgmpo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ciwovzgh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pnqfmhtf.html


<!-- 参考信息 -->