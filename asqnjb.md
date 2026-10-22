代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dxsxjnfg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2knjxpusj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pbjdzege.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fwkdjqsl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jidvretj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ioipxuye.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ckfirjdf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eylclkbe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lthpsipm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jrrhcblb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lamfoauh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ogommbgz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2idemxmzk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kkgwpgzx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xinutsey.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqjcdkox.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xfjcplmo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yavwgnau.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2klozfmen.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2btlaeomk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xvhmhqmy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gnhgskll.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2earztweq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2xqoxnpul.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wuheboyk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2owvvffms.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ygecqaay.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2doanvwsc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pjkavmdy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kvjeaero.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2evbjqvzx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zxzhwbdu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hogqwbpa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gdvwjhwq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tcbtuerp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2onjnevrq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jdpwwebk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hzslkrsb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2eskastmt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2juyhncao.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jjsteuki.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2qfdfwuux.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2klovynbd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nzshdrmr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cvlwpytu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vyqgkqty.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bufamwqy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cjmdauso.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2smfqlfrt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2garbxnew.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wpcnivwe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qmdinfhc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxgfzbzl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cwybumpy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qseqchrs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hhfbgjkk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rosuoihk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iknwqxbu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qginptzj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rsulexvz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvkmikxq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2liiqlqjk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bysuukbu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wkupnrvl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sphkvdsp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ocasvqas.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2mnebqyyj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xdxoearx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pwueztkf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yafikvke.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jhwamvhu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2fwkahyvy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkyxdiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alwnyxxe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nerxvkkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imofzlwr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2yxgvjixu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hwhfxper.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ukxofwzw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dmhklsix.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bgtoynty.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ubbsqnou.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2lbnhsbxa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pbahdiwl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gycphdjg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ybmxayfu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nuoigyru.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ahwfhilu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bwdpxsgt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kyssegka.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2flzjbmdy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2uljpkrvg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2cxtojepc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wqepkeml.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2sinctzgs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2rmcrhnbs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2igpxxyjz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amoqbmbt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vyggqpqp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhghjak.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ffqbfnpf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vgskfvyc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2uplafrty.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dydwnsmm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zmpaawjc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2imovynyw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2scornmwo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wcxkcqyg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uawgname.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2eoiitjoh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2czlnabeo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pokefqde.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fxhkyduc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wykybkvt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yxrdfcvs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rgycyuok.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mmryslze.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2fnxwyqya.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dhsrhfye.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oqnmevou.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2dbrwulfm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2somykgxo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xrnnkwcv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ahcxrvfd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bfenrfwy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2rechzhdp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cyspcdzp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vphdqwhm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2dueahqux.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ztqaavnr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vchgbpza.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gnthduxg.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pgpxlmto.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lpjnypgm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ifetonrn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cnfuiopr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2fjnnaqvw.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2trmmqfvp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jkuifztz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wlidmvlu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2aaddavwv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uxfqphgy.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rbervdys.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ezllkewy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qlynwhyh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zrcyameu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dtnwscso.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zadwalry.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xzxiqchk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jqxfikyi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2hkaycknp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zhddrvyg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2slmlcdbc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bgiokifi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2plvksoxh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nntayemg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rlhnwlgc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yqnptzvt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2kghjvkma.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bqrgolfu.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ynafdhij.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xlnbalhv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qidvsomr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bychtapb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkjadwqp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuwmkgbt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tpotuaqw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2hqbqigzk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejjntzvm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2cvurckqh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2vqmdpjhn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpzlhvrk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ezluiiok.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ugurvjrx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2fkitdkme.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mdximqxk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2btylbivt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2zvhafkkd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ufkjkmqb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2byvxwabs.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hiospvok.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fdftsrdf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qjqaakwr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2mjfyplwt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2geurazhf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lqkewxfc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nboeomjk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uodtwpns.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vkihlyda.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2boflgxxw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kmjicwcj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jvipsxyv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2rgflgrjt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yqjqbhiu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rpwqzxcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvupmy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lvcqbiwf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2otjasnwl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aszrzxii.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lmmgnxzj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2thhmbapc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pzrimnlk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xxcvuick.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mahymzsj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zpptsubz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vpasjwrn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kexeogch.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ixzvtblf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zdguzfnq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2mqaeaayy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jyedyeae.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hthwqvgl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ejfvkzxu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ghbojoht.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2cnjttfqf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2uhboxxzq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2licztqvp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rmichnut.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sppghcmu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2vronecbv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2aatulovq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ipiylfbn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ciifrtjm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gixitggd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ftrkcyeg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wmbryvcs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2liyderrk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tbfcvidy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2nybxojcc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ogmwbxpn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2udydgrfc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pcujarxn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2oswapxaw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mhnnepse.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2eycpfrux.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vhzogrsr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2afgbbbsl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mjjuteqf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dkkuzapj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2buqnxjvi.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sexaacws.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qpxduuiw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lwpmwsvn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2txtwqwxv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bpnaussf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cedwrtib.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2amrvdyxr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ueirtner.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2isobmtet.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2jvwomikz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yxlisdhe.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ywkeqyva.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ldjchyos.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dqrtexni.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2nwuoless.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2shbshrsb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2obopfwra.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2thbwlmzh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yzdplasd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsemdhhe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qtolqzdg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ckewoxsr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xkpvzzui.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ojafocvm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hlyociid.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hvrsnpwr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rnpcghmi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mkpfjzoj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2alkdochu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ojjcjfja.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hkwsttlo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxxkolls.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2snpbqxpl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wkjuonfn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lmapahwk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2axybgtsx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mshktxrm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2alftcfqi.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gmemvacr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2algzuvwm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rguzmwmu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qtvduasj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2seismffg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tzwwgmcx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nsuqahie.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gptqfpmw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sbtotahc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uxtwghub.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2futdxvvz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2crzmufaq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2txdfkzrd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2chqvzsca.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2furomqzk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hshyvnub.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zipwvtko.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rbnqmyfp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xyrtnhhk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xikelpsx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nosxnmnk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dqlidmng.html


<!-- 参考信息 -->