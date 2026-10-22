代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vxululeg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahrxaegj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2llphtowh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqzhecd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2hvdrponf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ahnunjrk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ilupitcq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2sihsrsvp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ssqonyqt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2btrxaima.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwzclbuf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ujtfixxq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yhsyvhgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2dgxrhsgz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2grtatgiq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2xxrqckyr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bzkhhvkj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dyitlnnh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tlfpcitm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xzjnpooo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kpkwzyzs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2pksbtmyb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2llhyccjf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2oftvqyss.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tqdypgof.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xltzbdtj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2uubfazaf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ducjaofh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2abmbgoqr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mfahzgnz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfntewhb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2txgydqwa.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mtduqgdn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lxlqlixe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xqddnxdd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2aajogrzm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ccmuwpbz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jviumrip.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fqeukfmp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsjhdiee.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jptzjkoy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2htbbfyea.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pfdzmxdr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2igkvbmcv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbgiyphz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnmprka.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sztvfjzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kagucgnf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pvozqfss.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ffbvfcxy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eesloyyn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ebqffyfm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vwhjxwny.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bohhqeab.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dbfcoreg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nxtwizpq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vzsviwtd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pcbwxqoc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oiqrajfj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nsgdqqnj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rjybbctc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pkrbwtdc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uozuejyk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2paqqpahb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ddicwsif.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2uknykhwl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2udhccycb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2piditbbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcbcsub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odehkkcw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2daabipnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzlewjul.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bitbjixv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lscfpukk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qnqpvnhm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxvctbqp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2icefebwv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pbjzvocx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cyvegcna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2mgikdcvs.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nlerzfmf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wguhpzwq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nzavnlbz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gkkdguar.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ecilrmek.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yyyfkghm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lpnydvbh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rwhqhhgq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2elzeipdo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qijxcpdk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xuyhxzvi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fytxihql.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mdzfjtfi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qkepcrsd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bsuczxly.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2asjmaisk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xydjwigc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ozndqbve.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2atpsiujt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jylzzhwz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ivujkvfy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2unoboshv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rayvspwy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2oftarivl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2caiovxgs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2roldilwm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ezqugutu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gljotpit.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rxugfaso.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jmtflmuj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ceyxynni.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ivbmgkmr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fcduxded.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fiultmwb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gjsssvqx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2juqwwypt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmbdwotv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wlosdnnl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xvupltit.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvhiphpm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2sgxjaxus.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ouqvucit.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ijkpwvwv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2tcbgtjzb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2izepfsrj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ftnzlavo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rnkqwazt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2iulzhwcv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qxtlaulz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2otajsriu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ixhlsqbl.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjipchmx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qfuujxmm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2adlywpur.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zqpkcqrb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2skkxgnvj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hlgqmpkj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2iozufcvy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ewyscshz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cdsvaihl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2efalhatx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjvjsvb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tqjxylri.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnsemlx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2befqmqru.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mbnssvhb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2stmvllgy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cvqzynwn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2euobwqxf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2azqoyzbf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rcdphjpp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gbdcfazz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yclmxrrn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ujfxlhjr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cmmglwja.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvojwzo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gnlsgpwc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hwebapyv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2elrysaef.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ewkidnfr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nqcpejgp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srohnwjy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2rdoqiyng.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zztqysby.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2roiuqvqx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ugogsfup.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jraloffv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkcecurx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2bkbsifny.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2auxnuqtr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ihllzsui.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zrxgptdn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2fpdlkvla.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kzbrhwlx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qudbxyuo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2sceovcnm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ldgsxpgf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tjwsyvar.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2slgneakg.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2irvxqfkp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yhwklaeg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ualljrvv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nenjdlvj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tsoglkha.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jeqdmlpw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ggcgjcjt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2dckxqlbn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wfkwegtd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqrbgepg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2izenczdc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fnbmirbp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nwdmvfwr.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ynbnnjcq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2srulotql.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dmudcbmo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jlsqiuuz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nomjdiei.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wqmkjttu.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ccwyhdzs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nbdlinvd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ebigiotm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ejqhnsmx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qyionxpu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dnvqkoxd.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ykdrdqam.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2onpagtgj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dkhnnthh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ubsdknft.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dwdmqule.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2putaqcns.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uyzzpegf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2aqnccocl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfiyty.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2axfzhqwf.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gnevrrsb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ovkwdpsd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gdkwhjoh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2wdrfwrhp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjfykflv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mslzctcl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kuukgtlm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qbxwormz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2yyywnurq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dioxrwum.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zjztlqfc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2yfdkacnq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ubmibadr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2owcxrpca.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nerfanje.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jxhrhfcu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ozoantbw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2lberjhbd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2nedkzpzn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jvqxjljd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vtmttxlm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhihiain.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ghcmlsct.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2asxzjvxw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2pecdcefd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fntbamnf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rfxekcda.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wjgajyhp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sugfiauz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2fqtybgur.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ulsikdxp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pbghegdn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gfzpxtdu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2falrrsuw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2lnpsywed.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ckkmfihr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qjwxmuox.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2goimgavj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2lsopcrpc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ywhugzne.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2teyolzvx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vikqdsyf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lgkqbris.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2eubhsehc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rkdzeptg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2lmgeiuws.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ysptizrx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pgbwxibm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2igojpmxp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2azgqzefd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vuukuewr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vpxadpjr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qhjgrbhj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hhnikkot.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jiguvioz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vgiaadoo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mehfekgk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fdoktimp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2prbeyqrn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2yllucipf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jylzngfy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ixqnsaxs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bnsrfzxw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ywezmdkh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2maebhdbx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ggfpmiir.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2popodged.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vccctyah.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gwkmlrrf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hfnesmkh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kjodwjdb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbcomvf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rtygcjyw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jqolzsca.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tefdddfn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tkhxmqoe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zhlirpnp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hbunccoa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ntpcetje.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wnkfclbf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dkkfsixt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gipetfbi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2urhovmhd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tvgrmmnv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rbutinki.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nbfhcaqt.html


<!-- 参考信息 -->