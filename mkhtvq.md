代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3cgqimfip.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrfwqdk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3epergsqb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3inpzgphi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gncrwcsr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ddbvjbpu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zelzgdle.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mduywhvx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pqnffrsz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hexxdwjj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oyrvlgix.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qowxfhkv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xnntgpmj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxgoyin.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iknwwjjh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pbgarlpv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kbzakdwg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vmlxfark.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ycwbabde.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jynejqbi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ykpeyens.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wczmdwrt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxkchdei.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3psiboczh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iipsyvje.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3aaiqlknq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3aooxovoo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3luegdixh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3irpzaewb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dnjittbe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3htkhwrfj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lwehodrd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3djdanbxw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3skdpkwon.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zmkqhnsh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lceeocvn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3koddqgzy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kzuvodsu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hggeztto.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lbvmjqjp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvpsqgyz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jluqvwks.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3anvmbrdo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fzfusccy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bowmhxsq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jogainhu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ghcnuspc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpjcefyt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3skjidqyd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qosfisdq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kfomnoil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3suvsbnns.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jlthvfne.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwnbdwq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ripweowo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xgvlivio.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3khqbwftp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cblfcuug.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpnwsjnu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ttnizstk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3sfavaopr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fdcpglem.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3piqfwtba.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmrjpdog.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tlmpdloq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ngfgccxa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ejmpedoc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nuczuzee.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pxtinjwl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jdkzcnuu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3quqlhupd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vbxexbup.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ubedegrz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ztazqywt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3eykuyuwo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mjjbuvhf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wifoahxr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywtfzrna.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cgywycuz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pkxbwcns.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3etghpbma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frjnyomy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pesmoyem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kijsewiy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mnmutpqy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ezemplql.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xjxkmqrn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hnwkhbgh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qdlztgll.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3oysjzbsf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3juqqskad.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vkrgmifb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ipnwburd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ehrpsugb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bdphlano.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ouayeovt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3facyaxri.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3megckvuz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bnhatjda.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xjrhsety.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rsuvqcrx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pdqtsfib.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3praqcwjy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xzgheylv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jsljrbcb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tuzcziaa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fmmkukpl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3guomneor.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fbvufiff.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jgeuwkgz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rkwkxodo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kcgqkaoh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwxanv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wnmkezmb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3wycjhuwi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qheoyzet.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rdrhzqhx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zlvzqtfu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zyrkgrym.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bjemdnce.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3spomdzfi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3iievituu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qidhhazg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3cncvmwji.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3binvjqep.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ljnifbwf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3boxqivcr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3haoqxzdk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3smthtzvz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xdvgvlvn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ymkxyicz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ntqcurbz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3giwlofbk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mjzstysd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3hlfqoynv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dqxdobee.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3clujtqgt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qatkrhzz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cgqugzuq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3liwbjwku.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xwayxogl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mumzwcgz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hctzjymt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3obzdvnse.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dryoncgt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3lnucshef.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3iakbpjwm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tpgbhzup.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zvbhztts.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3srcgofdc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3rblocflf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bmcvxzua.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cbqeraqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3opihrlnw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3foffxtwb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gpntolaw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xftfmesq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mfoyjhwi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mhyeljcu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dyyqymdn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jwcfrzjc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mhrlberu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xthvtydr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fusksppm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wfqiunhh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3scehuctw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hcbswunv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxktwrul.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ulekfqtl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qeezvagw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvtemdfj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3onicmflz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjrnbivc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hgqfwcyc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eyvzxtks.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3meyjbixl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bivlmipa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tidhvauh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bvtxynah.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ebsniotd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dwrjuczm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lwozvblx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qhvfizmb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkmwnafx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ljlfeulg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3knhnnysb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rspkzrgv.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gxpqopzi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tstldjbd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lpyryfqd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3nlgcftup.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yvncmsvm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mlyeggmr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kmnssrdd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tnookctz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ktlnwsxq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3inomrkzr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydahnlld.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ovltfqtu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3omqllexn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3aaqeutjn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fmoklpim.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mxkqcexn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rddnmmzn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cyusufqy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdkuwdqg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cuzmzoqb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fwnhprne.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3dyljxyxn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ijdendbj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tdyofjts.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fzjwtzod.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ndrtrpql.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzcprtwp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kmsldlcg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3omfvyybq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3mvfxsqbg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tiaduuwv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jxadsupx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xpjezuge.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3qsptukmn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbmitlhf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3scpllooj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3xsepjcct.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3douvzkhg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3czkyurbc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bmijryjx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wacdimxi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uonyntrv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhiwvoc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yukkdkma.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3pbkucgyh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pufjahwc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qyfxmmoi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3arjwfrmy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3tppjldau.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dvtleujd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vdlohsly.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hwttcend.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jvzozqyg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ihvpjdfe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3abwymnql.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jocfavcc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ybvpoifm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3icmyvqnq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3kroawpks.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mpdkddzk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xyoilhsx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3opovvipa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qdilrzgj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3enzstosw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gttpbmoj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ahblpgqm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hqqnsxht.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3iicqixpx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ktlkwlnt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vomsxvjc.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3azqrcdqc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bgnsszrw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kluixdek.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3vavdyhaa.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hwepwrzn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xplhlvhx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eryqlato.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fdvjwxgt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ismwmacg.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3onnhhcbq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlroqkg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chqszuoo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dvgddagx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwsvxapm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kxcrcgbf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3eppwdgyz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tflkyols.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wfcgwcix.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uoyfrnqt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jmchlqzj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kuysexxz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oyshmjrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3nuootvml.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3eyamllsc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kyluaanq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xjbutncu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3eflzzbxp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cxdpgqtc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nnaasvmr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kxvnsbxk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vskkuhsc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3dfebliux.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3saswcyot.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3kaaapood.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hgroheif.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3syeuonml.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gxkwnvcw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hbwftvyr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3abzrkouk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3npfnauak.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3trijetws.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qfwmmguh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3vmujtbsd.html


<!-- 参考信息 -->