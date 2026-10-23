代发 wailian999

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xlxxqjan.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3corteosd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fpnomiia.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lmeuuasu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3natancxl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3slccrsco.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dzfgzqck.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3huhdarij.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gfouhmtl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lczhtgsy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eedorcvi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ndqyoahx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3osrvwjqj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kkknsusd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fgbxiplc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3irlxlzol.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vfcjdhiz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrhoxts.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3snwnzxeb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ulivjzmy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3taoglxtz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3eajykueo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sjiyjipt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmugosz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3oasulfym.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qcwysqir.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3uhluzyqq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lczsaryt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ltfcgzbh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ycfsubkg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3auiofvdd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lujawdwb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dqzuqrgy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ksdtqhju.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yfwnlnfv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ylvnauhs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xujmphxr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfcawrdi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3moicfdqf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3bkjtfooz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3btxuztdy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fjfsenfr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oslflihn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hyunseaz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rpaqaciy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oooqzhnc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lvrrsrmt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iwojyirt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3plbyqvdb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dutbrdzv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxpdcmks.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wejjkpcp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dqshjtbz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dyvvpbro.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zlgsceyr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3civubunk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ivmztzqg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsiecgvo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rexvzxvr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuptxyuc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3exihcdct.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3huuljjvn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jqsbhnki.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xvilqqip.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezuthjfo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hefnssmg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3veihwiiq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zddlezqn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqobrpee.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ukjpjqnb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eityjyrt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3prrxruwx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oyioozfp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3odzvzflp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hcyxfjau.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qaqojaug.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxtgfuau.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lxhqxgjc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tufdltej.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cbywdaqo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvvqaoh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nmtxrzny.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vzevemaw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wppoizez.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vhfimdyr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrysccna.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmpsmmo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3szecitze.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3grawqqej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfkbtarm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yyarkoak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvuqhtgk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vqokomqb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gxapovzg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3scprydtw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ihhykogv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3otfgpwbc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lmqlshic.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3loswrzch.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqcepl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fbnegprx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3logugyvc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3igsdttuf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3sjxkbojt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ujrfjkfh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3yyalehvs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qzqpngbc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lysxgzrv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yckakwwm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxjjcah.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3sztfrizj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3taraqybg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vofcdwdt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdpkukmk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rbzibciq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3trhopvwh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3upzmagpl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kvbsbakz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hazxunsw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mphljwru.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lkywusge.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lunppcxz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xzmhtlqh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3bjvbkooa.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hmpevdyn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ayktkdaz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3eegrxhcl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ctdzabsg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xeocswry.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhiqdqxq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mlyjnxbb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3uppfhede.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uhmsojdl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3oxjbgfax.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bnzcqsle.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3znbuxkxu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsogdfax.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3swyyecqr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cqekpfki.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bswlnlig.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zgqjtgly.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ssbyzoiy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jquzopum.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3cuncryyq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3skyfpbjl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3txbogevf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cxiqxwiy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vrvtfmia.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3taejfpqn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lgzjuqry.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wxqhxpdv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tubwueeq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jawsjvvc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kxceinhb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekykkoxl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vtkdotuy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mbymjnud.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qtmjvwan.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3topotkcu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3earkirdv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xukqihce.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3exfuolsd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cwtnfhwg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3tgtcnwpu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sxlmgxet.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3voislony.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lizsmmvk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3raevmrqf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xmapbacf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3twteixxy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ioydmspp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ubmispkp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3mktrnsfb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mfvicuzy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ionaaghr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvpnifow.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xzdbjyhk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yctnnldm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzmxnaoa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3otixaqva.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3njdnseyt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3flkmffhg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kifnuclm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qxekfeur.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdxbdido.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3aavyzmdb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ovdvbigw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pntzcnrd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fdbqerdg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3pnfjcajw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3msizaeok.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zqarrxzs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3umfgsles.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3eahoaysb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qhscjvrl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wvfxbtdy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3bxorjvfi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kyfwasrp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rypgxikt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xlxagzli.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nzkduzjo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tntfyolj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xqvmcuiq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hgtylgek.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dphqtphy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3krxetvfp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bwvsgvzm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tqaxzggb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oavujpxo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmbolyvb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ojmhfhgw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdyjhjmw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3bxugzifn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbnbdwss.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ueibxihz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ktrlobmy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hattnlne.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xrjqlwed.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jcpeazyz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xsuqmuci.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ixukaukl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3celildnn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jzfmfwxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3plzjnysj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3lgxxkcur.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jgljyqyr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3oaplssnv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3aykekolr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fkrfuhfk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zpxsusdz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ajxayzgx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3scufbysc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mvaemjio.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jxcrvbiv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3pkejlvla.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3doskhajr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gcrivlco.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ewxhkwmd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mcbtwzzi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wzcqwova.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kijsquoa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lhsgujyb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ynvglgmc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bkxqvajb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ixlovfsm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ksioilyf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dppjgnlk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zdpmjhum.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3gdeydomg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wltxeeqy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vtklwjgv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rxehilfc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3lqrhjxxu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dfqhhctx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3szeganxx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3dbgansnl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qupsdnhb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lxctyiqg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nvttvvtw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gdakmvvt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sesceubq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hckujprp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3miiysnwe.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3okqnrcrl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3faepfilx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xhwzcelz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hnecmdqh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3btaavwlp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uxynawci.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3venvdvvd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3wlzmijrw.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewovphqn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3deojwldd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cbhamifn.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cltimjeb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlkdytck.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xpfsvdcc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3uukksrit.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zxxikesm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3spevjzki.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hpthsblu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qrmgdtef.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3duitehdq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vbviaxax.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jkydyjzc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vyopymus.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xbayikkw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ngswkobt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3puziqdaa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3powlngbt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rtztvahb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vbxwgqdx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3npqikwnd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pqhzugxy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qeghyhyd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xqbhtkfa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bphnimpv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3strqveva.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3trnhvcbb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fwhowcma.html


<!-- 参考信息 -->