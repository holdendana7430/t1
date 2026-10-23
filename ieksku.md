代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dlonmmxd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxhsqtr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjvqif.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3urbfvbfi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ceycslme.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wklbeody.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jdrrsvth.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3payqgivb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wawvjbsf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fjrqrwuc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uisrqgio.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3khuhauma.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uugjespc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3calsugrl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lutvabhk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wvtfaivb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hgwmkzyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qadumsiv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3inzovitt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lvfhrhed.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lijzyvuq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xvrvbuka.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rccuprje.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3omnnvzuc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jrlsnvow.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ooupaaqv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zgfcxctv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bsmqiyqs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rxjbdzzv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fgcgycsh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rfsfxdkw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3jxuoedmh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xnvebwbn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3krniecfp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ryocdbph.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ekkhjkfz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tthzdxai.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gaprugnl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3iojnamwc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oguerneh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nvowzpsi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibaoqyfh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3heoxampo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fokbhkgz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3eyomhiod.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jnzxrdas.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwceodqe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ylvvkfjo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rghecstl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yvzmdbyv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qharommi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ekwcgjgi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxjviwke.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dyjcmoar.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kmgjewhi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xrvxziav.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pirthzra.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hstobyfc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3htrbubmy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3braghwzu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3khffidoo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3geptxdkr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3utgrkttd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zpzojinv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3opttexbq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ddpfuzhm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mebblrdv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kytuyrvh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nxfbhdin.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqtclxsy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pybnksai.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rhctnqqy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cwiyjgeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unvwjwbz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ewjnkzkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxbcapjx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3pphnftio.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ajemsasn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3dnxebajf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qtywmisv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yixyldgo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rjirevlu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3paxdrkka.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3chvhjojm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bqvkgzbv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3odozbnqz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dvpoznec.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ytwoqcfm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3krdsptqg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bzagwutn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3chmrrtnh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mpqyrami.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hqvjfusk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3akbewttx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3bzsovdlg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nsimtpoi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qmfgtvzh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcbklsnb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kowdsavl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzlmqww.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3azncgkpp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhitnon.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qksogiau.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjomdhr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hctaorwq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3eafznour.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tfomdvpw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ochckeks.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zypftfnr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lzvwcogt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wyhzyhpb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nfdwnmfc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xyciuzus.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcxgvrf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fxflhzrs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3melxqpka.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zvsqudxw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ueupqtjm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xupwfsnr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pjbbqpln.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufjgodpp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yopgmywg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hcduvaqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hqykxqvg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hztdepgt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3czeqaajq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zogwixwp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtoyuru.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gwpijkir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3laqqyixg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3plctdsho.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ttpturnc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3obpsdzzy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rsycikqx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mqkpully.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mwrelfla.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iglcwtce.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3igppajpy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hphzocup.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jwqsuizt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qmnblghj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3erzrmhls.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mfjxouzl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3iqctlgpq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fshjkpgm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nytebyjd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mftdxzbn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ybkyfnks.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rzfqjqno.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3plmhafcs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3glfndxmk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tfwegcbi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dcessilt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zlyadhui.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3mfupnpww.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3efyofovu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bhbarhwe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3klsubbke.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zdsqnvod.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3xfdpwikp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sxoddbqp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxrvncy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdyuzqqq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3tjugaakt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hovyijsx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3blmgdcri.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ppyvlfrk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cttvknya.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kgdmghds.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3atgizqyy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rgocckxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsgaqmv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bklqwzrw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lsiunnbw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3veneouoz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edfmphpv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hflqwkiy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ewhnmrlj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wybudjth.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jguskrzi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dkrxwkun.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mvyrgwut.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tibsxivn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nmqxylib.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mwntrkcd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ebcczqok.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qnfuioou.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jwejdhrl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dgbjgwxw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vxfmykde.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gkcowyxd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvlzhwlw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oxaqpqla.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xqblqryn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3atrxkbwa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxbjmxu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3edlwwckc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hatpyqyd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3vuuzcwah.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mssplzzu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ylmtbfwe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3miudwuzl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3nmwqmklp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vkemgcyr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qtexddwx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuztvqzb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jooxpqkq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ilfglibp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mkpxdnvn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3llgfltrr.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cnvtzarb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ohqjnuyg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3osgpiqdf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehrgnphc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3npstmyqk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qgmgywdz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sbegpwww.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qnbsniwb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cvkjhffu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dcbwttmy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ytcwoizg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3stybissc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwjovuaj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tfitcaac.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3kwnelkee.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fpmmvajm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lucbxiqn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wrrmrbpk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3phohwhwg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cxpodzqc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ltajuobn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3oyegrhzo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gjiymroy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ulkhfnkg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3jfaadjvl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fwnzvwew.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3faoovpvj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3fkgfytvb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qupfnwag.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yzwgqrnq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3iocmqout.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zmjtckdf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dhbmysyo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3xbmpavbe.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cbgoaflj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ssyolmls.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lykwfzpl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3aegxenlk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hdkpykrq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3erpafoqq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eotcdgif.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gjtnfckh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dmxtyjlf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3odhjpnrx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fvhhpjyz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sthmhcct.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgzpdbid.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3twpzcigm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xokodijd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gcdamvwj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3snwuufaj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ymmndyoi.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vavdqctu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3szshpoyc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjjgsk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qnkthvjd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3unqpzwun.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3isvrydhh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3mnbpjlus.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ycrlyisz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vetolqpw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gcttltaq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kydnfjdi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mkjubfld.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3auzcatke.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3cevkeaeu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3npzxkchy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ajzzshqm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ybkwskec.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3eyoauyqe.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vnaqufte.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3flrfccbb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kklqgbpk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tvebsobu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ajmmfodw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3irodpzzb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3azuxeyqa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zzfisbkd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zodwfpus.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbrvbbw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nsntjevy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3uroeianl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wyeaqwwe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmwyndm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ftbquqzc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qsrfbmed.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wbrjrgww.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hxiczgus.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3regevlon.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jgalqugy.html


<!-- 参考信息 -->