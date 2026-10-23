代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qnrxhlal.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zhjdgrwh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lifeewtq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovmqhpdy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbbzycpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3acrusyxj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ingbiimc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvclqbeq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3iyvpcafy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvcbphl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uvbkqsln.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mpsfumma.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dtezdscm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vcoptbwo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ebmlihvd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uikndvot.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ltkrkzeh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjddyt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3whvgbcjx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mnlncmlo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jxhvtsox.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bqshocxr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lzcshzwy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlikdpio.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rknukkso.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3yzxcekvx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3trcxsgxy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jiuknaev.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lraxmyzi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bhlcodjb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tobjpsze.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xyfwadxs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qkmwtnsx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3junrrfff.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gfofahzu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ovwvvxcv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zuotaxvr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mhpxazmu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3pwrpthkj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bzjolcir.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qhvmgpiu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3hrjjpmfv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dsvvnvxw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gjjiitee.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yvxzpjzg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jpyqtzat.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rotytfzp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wgfpjdca.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kouhrgpt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkelktb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ykzuqzwo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3krnjopsy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qgxraxyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qogxlnzg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rhlklaph.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jsfjucta.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgedrfcz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sanlinxd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcuobwml.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjugnzn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmkufqgu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zughsxfw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mpshaacs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3arqenyvr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bkytrbjn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iaavuqhd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uyblsukv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3adijfjiz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpvfjaw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sqmvbsiz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hmgywfsi.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nfhgzsrv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yotysofg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qfieifov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uvuzliuo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wjvxrbyr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jzhsxede.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtgnhldq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gcazlqql.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvzrwf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oblbmsqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgdsxmfw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3skauuisx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usjxwvaq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hpckpuho.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dlizpnzq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vlgcjciy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqkbuztn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qzbekfoi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ycphzgmf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dhhdmcmh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bdxbytbu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nyrsxyip.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yhppeqpk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ckexrumw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rqgkcnft.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3uzpcgmpv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ngmltcoa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zlaiaxhg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3onyktblm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tbkumjrg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lnnjdupm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kegtenql.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hpdpwsvc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cbmczpbb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzxfzbp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3awwabydn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ouhlaogo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3llpjoqkb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3djtyakwo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fhvazwqd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3udtvwgbg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qxpolxbz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wvughszo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mgzisydq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3asknuzml.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3kebkvlgm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3svqynzhh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xzlmeoxu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dqcolmju.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cedtlaxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvsjdpke.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcclsr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3uokevpgr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tpgjsvoe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dyhzdarm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3rhontfvt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3qjjqofek.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vgvrxzut.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mcwomjks.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3tnyrqvja.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wipntpba.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3acacsrjf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ftgwtzjl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bvpoqiwr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3mrwkifmk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bmlecpay.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3egdsituk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cpnotfuf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuhcmi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gduebokh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hmdcnxvc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nsdxetug.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwdcnxx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3appzbyxd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pezqennk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3opxrlxtv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3reoishch.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3hmbvqbqu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eqvdfree.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3esdfljhy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tsvrtonh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qcyaditb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfgvkhz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ftazwhki.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hiytafhz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3liswbkxn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3iqhbslff.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vbeskxta.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wpbfzkrp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mvtgqmjr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qbwofuxi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tkyeeqrx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fkehaips.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ohljxlvc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vjsweknc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3scbvevbi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oawmwljd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vziivvyq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ynbvziqg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ucixccgl.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3oglimkur.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jfriaaqd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fjvstppo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ziaroqiq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ioaptuzi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3egpegqea.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fcfuczil.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ptuwwusq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltykctiu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vcywijjx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yinixwfb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kaqntlpv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nrsmpyvo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3upqdnaac.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3riygvyoh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gpsxoudv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uhcewxph.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3whihoymg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ydjhufxm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3shnkgkec.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nglnqabh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3efjzmghq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mkpxuogi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yycnsihn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoihtnxj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfqzmtxg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pgbzjwvw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wwewucfe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cdjavruw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dtuptqyq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jhglxyyn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3abclhdfl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dctxytpq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ehnozdxy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3djtrhkaz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3krpytqcg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xlhfdanb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xdtigdzi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3oqdjpomd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eczcgqxp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ytejqzwb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cmeyizfy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqixpqtm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3amezerfw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3elbxruii.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ttuxnbil.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ngixwmtc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bvoycmfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bbqbzzii.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3imqzgcyo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3dlpzbqbx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3urxjebof.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xlakckcr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3azmdrfdn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3adbrmrjo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jrpqgtwg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pzzqgafx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rkxyqhxf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3dlbvmhvx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xqjuelmy.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3huwwvhhl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zgmquqfp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dtsvzljz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ltsjrsmf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3fslxyswc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bsdrwbxr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nkjqjiim.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lgzmwxtv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3itfoiluy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ezzqomia.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3brfmyjon.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3eoqzsrzj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bpeeluhl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tuqetibh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3dgekojqp.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ogyhlgxi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bvejgmgx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3eblrwioe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3auholsxn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wuifrkut.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uyfoibym.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pslpxohb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fnpzwopm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3guqanknw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3usznlvrs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3drsehgov.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rxuemvvl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ozraxxvt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jlftlxnq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ckfxzvqk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gknmacfp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ubdiyfox.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ecusjjgj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wjnqnltk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zvbxswtp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zbavuswc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xsomahdb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3sokoosfm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dzysdeqm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sbjzbcxw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jsswfuwz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3emkugihb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3glrgopus.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fqlgasbx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xujzjrlg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ybyfxhht.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sqpzpwoc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yhccbpwp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jlarkrlo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yhheqhze.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nckoysmm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3oampjyci.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ipdhriso.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tnsqkjuq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3aukihshj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tobzwloy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3aunromuv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3livnqbws.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pstphuct.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3leektblz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xbonzepc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3phoxjzjh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hgvwndik.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qveczlmw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3irvmjwir.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bfosazqd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cihukadu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wwdvqboh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3acxgalme.html


<!-- 参考信息 -->