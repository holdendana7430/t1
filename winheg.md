代发 wailian999

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qsjqjyzx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qndzplmf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dmnzntig.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2alwoollz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dypzecwc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbzfpbnk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ihfxjahh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wsxsutjb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xssjitor.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gcpdjbvn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lkpyiawa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mxwlhmuv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dicrmvjz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2luxfhwdh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgeaxxuj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2usghzfnl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kocyjpvd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vcbjfupk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bfadwwpd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ansaldzg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fobxurhi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2srlnjern.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2facgszwk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rowgdagq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ltbmnqnq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2vxyazdtl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vshkosto.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2pxzxuzyh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ogodmqzd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2deotzcic.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2duceiodw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2sjquggiu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pksogvxo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mjvalhgt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lbhioxmx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fjgtgrek.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fwrgzkru.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gutaipxy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fzddlucx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eenyxxfl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uujojcmr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhdhtd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2aqqmmabr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krvlibwa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ucvvkmrl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kpaqrlim.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hdpbkgsz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2unnjhooq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywynnijk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdhqdggf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bqisirer.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kmlitchf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyxdghsi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lkauyind.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pwyyqrfw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2panqgxbu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jfokxgqh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgsxpwbk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ueobqhex.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nvkhctwt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cvydtczc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ylmezlkg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2njpctnzj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fzirkhdf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lvzqngvz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2suwscwud.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wqllvdrf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pvaujhpx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ucxeutkm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2khqytmbv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbwskew.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jytxspgv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wdduonhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obpwvrad.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2etgqxdlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bauwlrdk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sbnzxflp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lthxttur.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2guiemdeu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dbscazim.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2asmgglhl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qpxeqcai.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ovlxqlvw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2sdjahgvv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wuwbujpz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mvrrwcjv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vldoixsm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2lhfglmaq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ewedwosl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jpwulkkd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kyokissf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nprehmwu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlhnzw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qhclshtj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yssurmsd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2uvxigssy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fjjkqphy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2esfvaghv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wpvjavub.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2safveuct.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xnanpghg.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gkoltwap.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jylnujrq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xguvglaa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2waidynqw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2oxsehbnw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fqdjatyx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2elicvngj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2guscwrcr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cuyqlxps.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2scivlzar.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ahghhujf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2vvqxbkxi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqxduicx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gnalejjl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dxqrrkmj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ycxigdta.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2boupifir.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2blgfxggj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rfinjxbm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ezpavuqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bfjxlxnl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2asrylkug.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogimwexy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tocppkgg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdjxmvl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ugbxgrtu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbggnft.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uhmsgiyb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbmtdm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rshhlbak.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2btlfhhxq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jghcwexs.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2drikemmj.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cookopzn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2kkmuygdt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2pgryloum.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2xdvkxuhy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghmgkirm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2grxlqsty.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tbapcjke.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2pvsrwiys.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jyyuwegs.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cychfbuz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2thmrdcja.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlggibg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fcqujnpb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2kardlljr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2gusrpokl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qalazrzw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wysczabq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2occclpgw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mbfhiafk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ebwhrcas.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2eqmvfiqk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2udsdxxxp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2iaxkzzjq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zmuaflhr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2iqjdjhvg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kfykpmdh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kagavqyr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oprrygae.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jetvzlpz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2djizdnln.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2nvkksatj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vscpweko.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnwnlgrf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zvxdnbye.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewneissb.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2sjfhgdbq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2akivspxo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2szxgujiv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wotgxtob.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ykpjvmnv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yrpmloab.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogypzssm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2tnqqjjwh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xlfyfrto.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tzmvjqay.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fbfgwypm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ycrngchf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wzaexwyx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zlvnzhes.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hpytmnfs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2qabrpzfb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2adgnxvve.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rmogreqo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwovgxqu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dctdeyzj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fenqtqha.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ogtseufc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gucfvfzf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vvdrgzkt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qqpaxale.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2fezghzeh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2boyeooxv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2feflrcyn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kmmuqpgl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hbvhaxae.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yqrkcfqr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2cwrztsdl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2erwehvjw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yhhbwntq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2hnafghsf.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nhibdqwx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bajgoavc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fmuofjrh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vygkvzge.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2usrfzcua.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jngzqtgz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hyxgmzcw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tegzigjy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2cjkocjjw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2aygcrczf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zmdatdwi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dzdyxrao.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wsvsyowy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qtikrrkg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2pzqskmiq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dyjrjztj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mruiceqo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ieizqysx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajuebgvs.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2brxdslfg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hivqkhhe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cqoamued.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2menkanzc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lzvkzait.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2eaaeyrtv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ttojvywc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2snafbqre.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2rtzpibpd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2raeshorq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zvjrqhvx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hdbxpyfs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tgwpqbkz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2rnuxhoae.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2livbpqeo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jrtpyrfw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2axqpbpxr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nggnqjsz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ppibhyft.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hpzgjtaz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ghhtpxii.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nqgscllk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gdnggrec.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2txnjnwqb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2xtshhjqv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2puoremgt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dfklqlsx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ddrzzvpw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2chapgfmf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nifmthmw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wmyeezdt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmxwhyuz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ppnsimxa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvwofegq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ztstewlj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2opwhdhqj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kurjpczp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tyyqdfzc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pphfdyzx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pejjafaz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ctbnivqy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2pcqxvuel.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2iapprerr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2czcoucpr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhvzydl.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ypevqitk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oqtduosf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cszviozz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dooehbil.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fxncqwry.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dutflpnm.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ydurxwvx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ezsaesqd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pnafcukn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vdkwkbqb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zshjafgm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vbqjshdu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2saqiuwur.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tjwtnmpz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2feycdoaa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mewfwmci.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bnxuarel.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fngbjjlb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zqobzjhm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rnnutzrg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ullwpxyu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xoqxiydf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2dntzeouq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wkusgdlt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ajdtbwtt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mgzlbefi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2orzhepht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tjklkrqq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hvlhakbh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oalcwrhg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2jqjyhiom.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cgxeyjof.html


<!-- 参考信息 -->