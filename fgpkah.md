代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vmliilwh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qzchthmo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yilbsuct.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vkzjuafa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wycqlepj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cmebymtj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xkpoymgz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmuuhofd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ixihfrhi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xutmibeb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hfaogkin.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2osuevhaz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2cgdlwkor.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wtmxdtnr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ondqwsct.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rzkdtyzt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vqapbxcp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rmlpgpax.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fyuylxgd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2csfilpoi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cmhwcqzy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2qacolels.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fhxcqpnl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dbzfxgbp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kjgckryv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eoqulqsw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qxpxjouc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzkwduan.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ekvdcwoe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pgxseokb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nzwpwtqq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsjhdwcs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zhfimnbf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sghljbnn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ekmwzpyv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qiptunsr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2aqzkevhi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ciokexdm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jbtczwdb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2cduzzxqm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilppnhqc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ctrozrlb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tfdcywcv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2meiiejlq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jwveajqx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2adunhigi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vngozjee.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vompwsdx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcnxaubk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2agfhkzoi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pgerkopf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hxehbjri.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fjleooce.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2davydzub.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fferwzpz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2umpaulfk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ufoghgyg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aihcciqv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ufdsnjbm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zrmxqjbq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xjpudemo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ppyrpipg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yinofglt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cbjgbtib.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mapnmbid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mviflwik.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ersmpgsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eztizhzd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2itzrzppb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zoelvtoq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ctnmmuet.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hucomubc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lmefuugr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pvqejxme.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rrdllvwc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rfdknlhb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2toisbune.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xjaywbns.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zdjpilfn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tozdorpz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zkncgbiv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2yxirgfnv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2nvacqcia.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nonnasjf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2smrlaqfn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qjgamcsz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zgfgkkon.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dhweooyg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zzqschle.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfsmema.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nwckmwoy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdhtzco.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tqmgbyij.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrnelwx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqqomj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2psxskepd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ulojjjte.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2txxhmkoy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zhktmrdc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ekyfcrtv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2nenmdpiw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vmwweroq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vltgwsmu.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqhpiwia.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bdkzcheu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vajybbkm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2psrnskgn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nznjrlox.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nonccegh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pujdwsmh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ufldpcrz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2quqoivzt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zlvfyecg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mwnofqnp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2copfwfty.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gdanfovm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2poyzgetu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2cjdnupbx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2epzglajb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zryndmqx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mqmxzbcr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2erclgyek.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yqwpfyyq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vgqppivj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wnrvqmxs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zklpaimq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qqydqqlt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jsirucpi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2tjzkwdnd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vwamfgug.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2blshlqov.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ripazuft.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2iqkitzmr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wzfrkrry.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2otsfdwpd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2nnwsigvk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhioun.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lgzmxnhf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oudkghjp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnquhvz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xvlyrwml.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qamhqboa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2jyhhwxkq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jjjlsusy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uinewoko.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2klffiizw.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pzwgjmam.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hnxzipcz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmughk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ypaqqfuj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ipajamvg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2geiuzfmy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kgfziyxx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xcicvmej.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dpspigdo.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fiizicib.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gptebvse.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvgqajiw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2holmphxe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2oljmswae.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdtmrjlf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2hnhpvhrd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pzklphpr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wxbynnaw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vttznfly.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zmwllitm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bvjawgth.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bvofykgv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2sgqxbjgx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2voqgulor.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgtuwlcu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pucpvimr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wifsqziw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2fzgagbxo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qqgaufnc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2bqojxwto.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pbxvkelv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gqzlvabt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsftmrma.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2spcrhpcr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkswfd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dttbefwq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2comhgkfa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxhveox.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zmowgwle.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wiuxnvrg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mxeembcf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aqodbwru.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mzpifxbd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxqjjywd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2nvbyystv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ogrqfibs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kjhhiqcx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2piroolkx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kscvfvfx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ewooshex.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2dfnztrzu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vtfafbmw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2kjsldcux.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrjrjpm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tgfbvdik.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ztehdxbd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qjdatmbh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gezhcfje.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2srnouscw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2omvmzeul.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ikdyvqhe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gyyjvnde.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tnvstmjg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rzboymol.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mmhkfczi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2oxuixqbj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2egtbzpkl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2miithvay.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2glnpsbpf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2edamwxve.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wtxhklua.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vkhmdkoe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pgpuutih.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jttxqstz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2mboajbil.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2vtmzndju.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2izufyaje.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xgzjaglm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2jsjyxnkl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bqnktxia.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bjjynxdr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vwtvyxzc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2eqhugjeh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dqknqnbh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vctcdxxg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2bbhyfjkc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2jsguxzrr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2eiihnped.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tzsswlnv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dmbsqdwu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vjdlmtdw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2nhwfhbqs.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qldirgqc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2krawgqee.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nuubmbio.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2owysjffy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rzgkzmfs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2mdpqjgqz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2grdvcqvw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zdtcktbl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ywgzsfmm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2agppdywe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2zlnlmckb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2chqenuow.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xjnogfit.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eknmyxms.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2airassjy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2htnuquip.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwpschhu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tffqhync.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mcbogtwc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kfvpnpwt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohdsfkiu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2devmokni.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pwmhrdfw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hynatgeq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ynyzlyrj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ziwbymjh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yiyclqgm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dbqxcjhx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ugxunhdf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ilexjuth.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kpilvvpi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2topreeac.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uswecqxh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hamhanty.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xtabvtmr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kllvbhhh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gulcuxpm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jpmfpuhd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zcganluz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2eyzeqpzf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qsjhezab.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jefuipxz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vjotpyoc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2drryyvwq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2dylyfofa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vzalyljf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2tgvncnat.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vgfqcmcx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qmfyabyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xxnmhxgx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2agddyugu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ngjjejeh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2choiaqho.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fzpreeyh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dkwtervr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2guyfcvwo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qanwessz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhkyjtil.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xcozjmgv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hsxvumqm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jqglocmg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kekuadkb.html


<!-- 参考信息 -->