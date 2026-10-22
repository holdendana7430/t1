代发 wailian999

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2valyzgzc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2igtahuqw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2trgjynla.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ifxpwzqg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sukqyshi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ehdrzfde.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nhtzjqkv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uwqdqzet.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2moykjohz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tzbfwawd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bnyhyqht.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wgbyakiq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2swnlmflt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2joivznun.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lcyxemxw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2thlilbjj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nwdntzyc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bvzuowsf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbsnzixm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2azmippip.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nxsxyodc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ljrxqwwy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xvjstiep.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2knklahru.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vgiebqhy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2itoqpkwu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2botoeeit.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2iajeezba.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vfjxiqem.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2zfgfifce.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vnkjnxni.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xofrsnal.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ndvnaouc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mrpkodii.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bljedvlx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tujbryid.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqzbuxkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vvbcqcgv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nabpnlgv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vodictty.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2udynxflb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hniujfgh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vjfvlkee.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhztleph.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2skzpgwxt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bphofmmu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xkchsgqm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwtszpr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rmcsvfmc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pvvgbcrq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ttnzjjvz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2koouiwdp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dmscftwt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jbzsnlch.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbzwqflg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qtadhenh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2glhixreb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ffxpmywg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dmonugdp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xwzdswkw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aivcwaoi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2krjkgsgs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yywrasqb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fzhemrlu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xohcpiql.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vidwhuea.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lbfwnimx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yejsyckg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nayemrue.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fextzkfd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iajfosxv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2eioaxlwx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ygnnaykr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cupxclav.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmbvlnk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2randuawu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ccvbaygd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvihwofv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hmhyqmsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwvauror.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dzlzgrqg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jrmwhugs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zcmkizhn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2urqhzxhr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ybeybkoa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ytosnitf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ozkvrzbe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kapckxpx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ftrztlwy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2upjjvgsv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qhewqzrw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2oageyxww.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2elclhexq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wvowyiiv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2uxfjmfso.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nyqusczp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2raodrrhz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2guzbtmhw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qhqioozj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yvyrpsql.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tbnaabzy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2njteduzv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jghueyps.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dlqqzdbq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hhiuvlak.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2avcjmhhs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2viunowax.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bntoyjyh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rjbmsimt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lboqfzzh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ktuglxcm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2crnrteon.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2oukwhfoz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jrlkmgle.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2woavrdfo.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hrziigkn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cqqjhrhb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycggwqfy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ksyeayiv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pxtpsufr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rrvwplwg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nmprwndt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xerkljci.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2yvcylkbc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qlederxq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qbczpeiw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2njxpqwgr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uwmgddfw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2suckasty.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pbywsiev.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2hrdjbxsc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxmblxw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2iuflkjow.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2oamlixol.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2tpnxbacg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2sqersmxe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bgjcgcdn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fhqafbdg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ayzycvyb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2puwgkxla.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hnrcevgn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zyjathup.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hbrbajiy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hlrcvzse.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2lmxesqgb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2omzmizeg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rjqfnfbq.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vlrixcgl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ifhnbgqf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ghsrofgy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2buzoafod.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xnjkyarg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2sbquzknl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2lmvfmtww.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2pskngvbb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2lphraqmy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2meslggml.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2nrxmnvbm.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zvuenkdg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jmcclfew.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2migiaper.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xeanjjzo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2vjbnoolk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vqfazkyq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hzcneleu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2bflbzvcg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gcjwkqsx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dbhtpymy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2eznyvgxi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bmbqtkts.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2waxdqune.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2waoygioo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jrcbzuqh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2skehfcri.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cphtbuim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eismergw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kwsscsgg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ttktcpde.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kbvbqzdu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jdounqqi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zilbugou.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qqugsayc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2opmpbtlx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2msumatfu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hucauvxu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lixzckyp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rmwagrgr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yodswbvb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xvvcaxff.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tnwjwhiv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2hlsozyyb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ntmxqngt.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2shiaqdzz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cbczioqd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nkecitmr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ehtcbhwd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ytfcdsrt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gdnydtid.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ienpvrha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cdbhxyqc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gowvfekk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mgewsxyh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ocfygylb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bpwkluuw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qzpwdsua.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aparpxue.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ctcssaeo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2bvcmxsff.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2czmcvgdl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rlutemok.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ixsjqmwn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2njkyqgdh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2btkbhaqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qurfcega.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hiqhgyab.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ihohcaev.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2agtihzqp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dhertwpy.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ymyvsssf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2eqirwmdu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tclgxexc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hfqvbxqh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xqmxzgne.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xrykgqyk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ijvnbtsa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ofnwvgpx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mtfdorja.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ckgvamxj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tweeocqd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cieijqcx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ljdlhrkt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lwjogaez.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2artowksq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fphimdan.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wapvioze.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qsbufcci.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ctnhqkuv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2anrjarqn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rrymdhdc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2munlwwmf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2giomfwen.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ncucphmq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zlufyhfv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqefwxq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vyxbayqq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dysmxpgb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wvysocnm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2vbqklvvf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ucjltmss.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vdlngetk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jztudsef.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ivimaval.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tolknfpu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pkwmmiox.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mczapbff.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2quvzikvw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lqxyzcru.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rqvndnsl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vurzffqa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtwsxxwp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vglfwyxd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rlznqxtc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mlupewns.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffzgczlo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ddgdqkml.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cwntuhbs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2scixaphv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ijojnkmp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lcxkrzll.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kutqketl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ftgcuxlr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytagnygs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nkazuffn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sguzgwel.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2earhrjtc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qnfmeett.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dqnhugjs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2tpcyftmj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2uomiwoyk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mnhpdudy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jzdprygf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fxhwhnee.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ocuhdfua.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zqifzujn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2shgvmxue.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2uqqroypo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2aoqpmefv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jhhnnaws.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xiajskvd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2flguboir.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2epdeawhu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2feqxielq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dbiyjqlm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbcixg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2obdfvvvb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yhypthet.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2auzflimi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kkmalijc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xcfxugwk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pckycvxx.html


<!-- 参考信息 -->