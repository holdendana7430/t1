代发 wailian999

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2uepqzfec.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ikxmilzo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2oodbnfds.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwrjpwsa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cwcydfca.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yqixacni.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dkkwcfhw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yauxwxcw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hmzeldpv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uspqcwdh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pdemomll.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2edgvdtnf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wylmgtfe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjctfjps.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bnyvflkz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jaykxryv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2plzuldba.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2itfmeden.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bmrqgzzm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2sxrcrkgq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tgktkkhe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kemvihwp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mkyipgjz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vcgoheuf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fuwlbjjr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zgliywxw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lejxuuuq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vwgveuzb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ecqqjerp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2amcwfzxs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mexapmgu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vbhvevxt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2esfeyhpm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dpsmqdsu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mrdeqatu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2azxghqzt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ykiuctds.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hvkcuwiv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fatpmqgb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zajfhghj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2clhldlhj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nqbtwtwr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hwnluezr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjvbacr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ikmxmxln.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vrvwaxjq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wewlfrag.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ievyhial.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jknnjikz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmegcuow.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ynmdebsz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlztjxw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2tkmpwnju.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ckyudeoy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qszszaso.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cnhzwsov.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuaemlot.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujxnzexj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qyudhxfv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xuztskzt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkzgxrcu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mepooqkk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2syezjgwx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2advlsavy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jcgmehqe.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hhkccdct.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jcejgcko.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rqsmgaos.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tzzgrkwb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ngxawpqf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fycfgcjr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hygfkplg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wpzagazk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nehpzqhz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2glnblusk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lhkjgsck.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2koabbwrg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qrewehmd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ksyvxvek.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2utnaszvj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2inxteekm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdjxbzqt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ypszujbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hamufdcw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vzzewzwq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pruscoxr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lsxmpfjj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bacjcveb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yfagdyqn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2muwqkoki.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ootnxqra.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bhllduzh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bqgeqysc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rrkdujxj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nsgpvufe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ydfcpqit.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pzodrssf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2uahujzjv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jsmimikl.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2smubmhfb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yqvwlkuf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ufpowevm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wqxqutso.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lxtkzqpf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ddxqeebl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdfnzjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zkwjihbi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmgxjfg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ivtpbmfe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqnqahx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2glfmuwtp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uenvivjk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jfztvsyn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fnrcbsjo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2avwyacru.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mdnimdyk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hjrtbutj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ysditkom.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fawqftew.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vhwiucrv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fzehdoie.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytacitih.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lqcyfmcs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2mliwqfwe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wnsigena.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qmdvbfqt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2mzubmwnp.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bwxrknou.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2doitellu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uchpbqeo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jytudppn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zakwgdim.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ceagzfdr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkedkhb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2clrfrunn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wimibnku.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lvjczuwc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ofgkwaow.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2leclsehm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gjycklsa.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gekckufw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pkwqphfr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nqmttzqs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tmnmsxys.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jkvnoakk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2slyrgnvt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eucubrsa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xfxvgonp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2crsvlmev.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jahdpelx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2oncwtjjl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fpxzflho.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vvxlhoeq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2njcvziez.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vbsgbefr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rzinxlds.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jkugvmpt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2aynywdbl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nblziawf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bdrkpyqa.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2otxveowm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2olydcweg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mfxqxzoz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2djfmaqvz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cfcyrktf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qxzequuo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pccjxrxz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qjkdpowo.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2cetpfhll.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2shhjxagv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gigyqwqg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jgepqzjf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2suxcruex.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2koetjrwm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qfwptvcl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2saivmtpb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2aaogiabc.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2matkyzwv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rdpfdled.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jqhmnayw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hwbkfqzw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ybwriffm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2drjaxejx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruxttmiv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uyvygwoi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2iipiwomg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgjdzzgp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nqelhglk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2dbwmpzfj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fidffpwr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2mslpgpra.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2irkqpmhm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2anlqinkp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dxeoqpbo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vdnmzvjs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eibxjstd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2omoczaos.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fbxvzspo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2unpemsfc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2trncukbb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2khlqgisi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2czeycvsu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rzunebhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jcijapkz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mdvhcxvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xazwblsn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2obhngypu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzzhned.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nyruztgz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hbpaxcoz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2krtxjets.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2siybbtoy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2oeseknlp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oedfsjpm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jcowkwdk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2onobbjvh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2bihllitx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2bdnbuolv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2rahohjlj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aobgyuea.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kminlvlc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2dcmgceez.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2lvmimvxz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2slydfiys.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fwvqdbvl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nuykamvi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yvoheqzt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2mikqoqfj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2tnibsqvd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bygpmnas.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ojkyyaoj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vqoffrvi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ekfepwbg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nxrgylnd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mhuvjuzn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vxhuhfoo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2agakgtxf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bbbrgvxl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nuxrxpgh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2cmogpdbp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sngxrprf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2murmeqtf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vpduuhds.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xkkfjyie.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2effmsjlr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ysedgwgv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kfsmhvbt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qytwiylc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2sokgzqxx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2paqbsmzm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ifcfzssv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nakvkfwv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bqtvfspl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gposssym.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rcrfprev.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jarkqwfh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ncncsoyt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2iyxlyghc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ysodjvcl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dhdazmut.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tatczyum.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pngjwyxv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2spqwfxsd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lzhabwdm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xrlmwczk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iwaghxao.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rdpubpev.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qmfldcox.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxkbcabw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2wjrooiir.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jonjdrzp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uyvapuud.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2acbnlwwi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lzskbzwx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zvzyqmpz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhoqkebs.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2gutczzvm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nbkiwppm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2apwlijtx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qocffzwz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mdmibwcw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2efivfavy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2yfqknnzj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2mdwpamwz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbixsoap.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvlsxvq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yqotakzd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2lfehjpln.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2fsovmefd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2trjcwuvc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bohiulmg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vvmwiibi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2iyaafjhb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tizcxdqj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2anddzjiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nsthrcne.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2omlyesfw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dinvysnn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2mgujblnk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2uqkeznoj.html


<!-- 参考信息 -->