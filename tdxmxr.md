代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3brgycbil.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vxsxpxxs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3snngmtny.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3mfoljcpf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fkvxgimf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jckaltst.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ddszkiex.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kcldylnr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ltgonite.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pqudlweo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kjnradli.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jbngylxd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kzixdyww.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3darulgwo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bphjyqqa.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kbpknhgq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hoaiijmc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3nywdgeho.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3stykitgz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3lqxukpnd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ohfkfcno.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3usodzlbf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uijvffss.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3omzrauar.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3votlwgdo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nuccjfqd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3khmjksco.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wkntybdv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xqroapak.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ovhcgsho.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3llgxlcku.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qtetlcce.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fexioghz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nkigsixj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3defewbna.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3endknmjn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3okxjftok.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lqvdqclu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fthmqojz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eekctdwa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tafllynw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3nmfhxoje.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3clkxtyao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mbhexxzk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3juyhyhcy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nbuvusod.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gvtzokgm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bahfsfll.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewliczvb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxisyiwl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dcjeabnj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3osljtjru.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3upvoeiex.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbbkqrza.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nifmpves.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhshsmtb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ssosllqs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ptqncmzp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wxctmqew.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tpnzfbhn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuouhftr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ogbetjoo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3naabsoca.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yyfcailf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lkaecmmh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3djjaqjeo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xhouolsw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ipjthapc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3pjilfksx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ludfrnga.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnodrql.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3aevxrbkr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3glfwnxze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orafwoxc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nbilitdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkvpdcxx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3obzqudjp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3weiqvrew.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zarvtopb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3udxspsmr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qtezyxtl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qjmfafka.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3juvisxow.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3novhwybg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tvlsltfu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jaukcfuz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hreourcb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kjtdeisl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mluwxusa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3gbtmtgzv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qopsgeam.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tojvtyys.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dvkfezsc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3byfvlnou.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pvkfzodn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nhxfjmyy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nlfiltid.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fktajjli.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eqsuufcm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rbyqhazg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hssegckg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3opgeccuc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rmnvxtuq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kihfcbtu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ljajmlim.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3swuvharh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zilxgqgo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jfewmgdi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qifujrmy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ytpvsybm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ujqyxszu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hxiopiia.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ynnohcdi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3exxuvkhs.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3fffqvqdw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dwwriyvx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gjhnbrtx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jnsgkjyo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3myowlukf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jrsuvayu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucyptkpn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yojlzbvt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3olgwezke.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzvgzqb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vygbnhdb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ulctedyj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fysxaeut.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwoxjrx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wbjcmmfz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tctjigdb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kuutcuwq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wbtcdbrb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qmvglfjs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cxjjleoh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3sjrbtwqc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dnajmxxe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wkwrgxgs.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dvgsjkjk.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nkddgiao.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3efawcmze.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gasfsbec.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tflkqdjr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3flfooqfj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3seymbvso.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kjerdflr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvditfi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rmfycqtx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gvcgycwz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mmpaeicz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3mtygiace.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3akgglyyf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gshfcgge.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3smrksntg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qyzpcgar.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3doqvrqtu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxqivalo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xlcaxuhu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bonldddj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ekngizdm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wnysmfyz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cgygjlkp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3gobopvij.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrnizpui.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vwawaxov.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xrzejkwu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fqjxsezt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3migljtsf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lhqjyvlk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvxllrnn.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pyzdskfg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wrymcgdk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hfzwxyfu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wdbrutyx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xlzpidzm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nlktkimr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nurzmrgd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3shrlwfbw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jobjtirl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xiwqjmem.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hnzgukms.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dumbsgrb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3yzosefsu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ebuiimqt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3htkzlwab.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bbseyaia.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uvwvumts.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hunalwfj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrstmqb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dxvlogta.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mwhubveg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vtqbuoju.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dovvopld.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qsdlsdgq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xjnygcou.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kbxewbis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lseiyfiq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jdvwkqcz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ybcgqfix.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nkcknktp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ygvpsbvc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3psbtkzhp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mhlqwfgj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aecjhtzc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3jsvpboxc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3eppwprdp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bhnvyzvg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dcjprgtn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ayzdjtgd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3trqpnpdr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3enztmajp.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jijqekxj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kerggvda.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3afdaxlpm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ihdnejls.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gfoxmpmv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3blrxajon.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nozokimb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ekyrbihq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jjfrfpmk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qprajnrf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oqaqwnbc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3djykzqas.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cnyccwvk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vnxgkbem.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ynvzfjxh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qsmfxmcy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3urmyhoad.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ysbvallb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bzmxxuxp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dohozxhy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ehntswfz.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3cghaaytd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mboqpkcf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3djxlwblz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sdvgaepb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fsvddroc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fnewwwlz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vyovxpdx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wuihalvy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zcqkzclk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zfsrlhfk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ualxcwvc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bdyebyfu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qbibzjhq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yrsksdhb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3uvirlzgq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ktuteowt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wymkjgip.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vusverjk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3egjskqgk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nksmisoe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3urkhontn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3olupwajm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eqsqknyb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3agwcojhy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzfapuk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kstihcis.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gwmyppzr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mfvslmef.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hohcltfv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlzcgnma.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qxnhozpr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucidcjmi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3owgpydqi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hjdwmaxp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qctxdmrl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nrgpeeuv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jefbtdee.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3vurnplql.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3glqimyak.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ybclovoj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3htgszjyh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ltnfftqf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3opwvajpr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3gyufnprk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ifalbwfd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3reifzweu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xmglwlkb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xtdknbcx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hukngjmg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lifsgqzv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3istsrbgk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3atfpplce.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ittiideh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xzokzpfe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cgkqdcrv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aeybahzm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yglhibur.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xoyctzfs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sabeqbjq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xemktxqk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jvycxotu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gpuvvgvw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3izwbfpjn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zbikaogd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zzgohqxr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3nyieqtqx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xrialrel.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rofslpjb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hxopxers.html


<!-- 参考信息 -->