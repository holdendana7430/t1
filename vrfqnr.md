代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jhxvgkqi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kpmjbgxi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3bjkuwplu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dawhevms.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzdgpuxw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvasfji.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3givhrqdw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ugjtzkvk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sbdwmzaz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rlhiwhoj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zlhqgksk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cazzhgcw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sguzcghs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3soxtnnqm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3afbvupbk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hiqwehnv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3doizmaie.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfgqrb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3bdjmhecw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gxgtkvmm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ffpsumih.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tvjfggrm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gxjnofkr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylotgdkw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xkjcrfgd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ojwevgmo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3iccumsik.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3syggdtns.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3arhxndrk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wotpivtv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rpevdojp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pzarzbsw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cvepeaet.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3icouobio.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ixcdyyvh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3aiokanyg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nxtvynjc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sklipgix.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zhpbokmf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3eiolafdl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ausflreu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gaieeneo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tuqafzof.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iezpygav.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfpdhoqr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lspvyiad.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xmtfrcda.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvakbwf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xqkidyhx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwqdwyms.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dwdzbnhn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yzwbuqyv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wlggvgqy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cacusgzz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ptjqbyys.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nohootnn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3clsjdapd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3retiktkx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xzkbbacw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3npmjywjq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3frnkkfpj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lcmwoeal.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jnqusszr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xhdzrdmo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3odfzsrbm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fekuhclf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fdjfyeqo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iasmjoiu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vmlutdbt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3legsgrif.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3pwkmneae.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vlcqqfvz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dxftwfuv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dwyvoagc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hzcizfdj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dswkphwz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3yxyeuzmb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ntzzdzgw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pillhwby.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xakrvnya.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ycfslste.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itvdbtvi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylciqmov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czerffzz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3oiivfysy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oritbjvn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iolysvlc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zbxtftyg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ubcitrts.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zeliygyk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yequgmsf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3itygopqu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bvwchhjq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3urjmbplq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3durmpger.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3msdypyuk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gdnzaztf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3uxjbetwa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3iclrghzs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bpxxhxsb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3srknmznx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wfjwkiry.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rqheygdy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wqcgrgkq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3pjlugzcv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3voffvzdj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rhzaowvx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oaexcfwq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ulcshjbs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3sydddwad.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3trbbhexn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bshbozws.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jigearpw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3anzaocyc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3iurtbygl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vmixmrvq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3aktirdwx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yjtpzmnz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cjwxknzw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cqlwbyui.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xjiqcuzv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3nvcimfso.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3isygnzrt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ormijcfo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wrhyvjfa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3pvjehaqg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ujfibffw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3klftgadw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3krhcbuut.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ikiaocws.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lvjpkcok.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ebnxbiqf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mqbhhizu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mxbpmrwl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3bwouprle.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ljxeefuv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bhazpwfc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3cncmjtyv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vaszurlt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ivbfosvk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ilmnbido.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3iqucqjen.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3krukdtwa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cplcixkb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kuezefft.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dsitulyc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uidesiik.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lbhvhwab.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ovwewogd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qvotfbtx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xzkouohe.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fchtkpua.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ayhapliv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yptpxeib.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nljbfbpd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3asjidgiv.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mjzlfiyp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vpbepfvo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yzwegvoe.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3srbxxoaa.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3uhprnbth.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rcszxvfv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ggnfoovp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nayqwhai.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wvydfowz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mgmtzpxv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ojapgegw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3himkvfgm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rfzcfyxk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zmrzhbyt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3etrsyjie.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3drnnkbhc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jkcegpgg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rzdxhxvc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzaqqmlc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ebhgclfe.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjvjajzz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pkamfwdz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tgntqnms.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdgwqiic.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3erfgeove.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3puhxuflq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dmzhthmr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujtunttg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3upoxohbg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qtcvvmbp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqeooofu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jwmcullf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3tudcemsc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ovrfdfsk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qxbgdhjh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3otxmbgji.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ygippenv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rjrsvsvn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wiorpgtn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gqqqfycn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vmsmqmyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3silskmgi.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xhiprlpc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3thmlxzpx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ohfnjyom.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3patkmqkk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3mxbxtgub.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3neayvcrp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3aodvwrbr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mqefvwza.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kydtymfl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pjazwdwt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mphdmzsv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yumaqstd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pytbcaix.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ckaxdfgx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zkywxkhr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3msxwngua.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hztlvhfh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3dcnzumam.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3redmeosi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iowwtpxr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ubuqribd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yzopyjpv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzrybxpi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvhjyisj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3udgvvwkh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3atgacims.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3udbfddly.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gjacfyzx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dvqmudpz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3lhgeiolk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sizcbhuh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xhyldyab.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vtwwvjgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3bmdjgjem.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3otkmjres.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3icgznqhd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hxtkiwhm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3oegardgs.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xjqgbltr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rdurisrz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xejfmlle.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xykhqlkq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rcunxjbc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jalelabn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nitklent.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3otspfwko.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3sqvmpljn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hstwynyr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yzlhqois.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3owlnqyei.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ucvtccqs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fsvkunus.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3fohmbdir.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3anxomyak.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3xkyromjz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3azafxglq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3byrffhxy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3grlbhvmk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3khdbjidz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vekamyos.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3xgqvpdto.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yczdidiu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3dozvrnuh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pgifjvxx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mraapdtm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bngjjptx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vcbrrsqo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zgsqfqlp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zkzfxidt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcljdkn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wpndchev.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dztcvjxq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3estujelh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uymxjvin.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ftwrexnk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3abbyflgq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3liocahzd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvwplnt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lmzeyaaj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rgddskup.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kgcrzdcj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rdzfqzsh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xpoqgflf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3umewpvxy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3cbblzrxz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3werrizom.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dwenafvv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rhsxyyxf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wltlwcmv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rgpcerxe.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3khxdmavd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dchgayqn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3khcmaycp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mxpqqdlx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ikldiqyx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pvorduif.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hodoirsc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yottzswn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qpvkqomk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3abaseltc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qqyepmbw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vrstdobx.html


<!-- 参考信息 -->