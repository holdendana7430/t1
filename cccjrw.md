代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kwkxllim.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2inqiobjd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2axjlrnnk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2pvhstiet.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2elyueakp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mdpmxeid.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rghoqgov.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2hsztncgx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mctwgwao.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2slmzhxqb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdrmsfvc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzrrmygb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2osvsvouw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xfsuplss.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ofrjmipa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bwstayzb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wnthmerm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2knwoisns.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukrzvjmo.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ohcwqkek.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dlodbpod.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ujvvpshl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2beckogfm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2noobzvqw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtncbkmw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ydvdqhlf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2bxlaetze.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eobsgexw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyznmhlc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xdvjsgjf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrhabkgx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tgsivrzx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2inctsqtx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xjwtwfqe.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qociqgrx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dooojtqm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vmqdzgjk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pupwiqoe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tzwmndkm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfeexnx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2aepsxwaa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nklxylpv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qeeyactx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lmgaunoc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2halsuyhq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qshbihda.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2emrsjrxh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2cwjeanod.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2clvgfeuh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sugemlng.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zowgoacl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jkwrvnfr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lvdqvqqu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gatookhe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ddrepvor.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pmmdbiyr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2scbhpeds.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iakffhek.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2grelldso.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tpscoevh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbfqtyx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2yaykctbq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ffwguwus.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jnfktlxp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xasznyhe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2syfkuycz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mnurlmej.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qsocbsjq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wztbyzyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tinxuvpo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yirxxbzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uslbglig.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mhtkrgps.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2oktytenz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2hyjspcgo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htxwyujo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uofrjfaq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bcxdddtt.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kpzsjrxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bbzhrnwb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rjkhoojw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pfckosmn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rjutphme.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2alkevhlj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2qyjlotsp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uxxymtrk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lykvsedd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zxinqmbk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pgnbpfvy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2khqqapab.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2paarmflz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fszgzohz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pfhwffdt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqizzov.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tmricypr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jyjtigtk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vsoqsoxt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2twckwjco.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zrxzskri.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ekckcber.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nhbhpatb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2vuqcbldv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2plodendt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kddfwfpc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2llvknoub.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ranccfwo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vrwulmvx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jckscrag.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2syafqjjp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwezaevn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mvcvlzid.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2avzivxjd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yittiawd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2weglosle.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zsxelfdm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ffgpxkgl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zradtufz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2xdlueyvn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xgwkyotu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jxckcjzd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ijuqljkb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2wleqsqrh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zgddobab.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nppiwbsp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lixqshix.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cjrctlqa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rcrlxxgb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2poveacoe.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gmneftiw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qzxwenzw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vimkbail.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nctzxfjq.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wtgxvway.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2skplypbe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbwjigpy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2iyftkqox.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ixxouhyf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jsehupvj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lqedpkqu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vvtvclcc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nwifxxap.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2totggwuq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hduoofsi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2crhobjes.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mwcxxqig.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vysgxjqg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2akpqeaep.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2bjcmqtkm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ufehkfsn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vgmxxyrg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bevuprmi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vsecixrg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fphckjbt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rmvrwigj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2yaiyyruz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ljtbslun.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vffajqbv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2grvpswgy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2selryerf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wddmakwp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ncjjwfgx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ylwcsjug.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2kivnyjnh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dkieclmx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmhgehlr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gtjgrvsg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gffjmfre.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2anqkwcer.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zmqktntv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hopizrmh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jcrnqsrc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2sootqgij.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2smpvqyfh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2mriekytu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mjnxjuhz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wbnwiwiw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bapmcipq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rmiveggk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wjkbuvdh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2fdpqtjcg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xpqunxiv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mkqasvhs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qfbmxtgh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqklmjpb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rnyqefxw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2busvkonb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2noacugkf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xoewupst.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nfukubpi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uapinlkf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ywnepayo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fobvevik.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2txacnjlh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iyfdvzcm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zbrwqfuw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2aovtdoos.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2huitffxr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hgyxhkvk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kbamrrqy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2nowembqp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2jsknpemu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2syjfsebt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2epbylmzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lphkfuoz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oistkdqy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pjdhwlth.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dgkyruvs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dbtxlksy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2wfvzsamv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhsgfehg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2nxqthqzb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2lfblgvtj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjwwhz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vcikyntq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tftgqjem.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jpbofbiz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hdwzaaxu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gpjrwjvo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2himvtnpf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mvpohxkc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2isghbnft.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rcfwswlw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yqtxhdut.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2djknadvh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2sgetuofg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jdonjuxk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eumiweiv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jnplbkgw.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qjzfpdro.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vmwtcufk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2widsinlj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2knyqbeyx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2liwecxsw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qamcgfmk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wdlmwliu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mumbjgrp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2deejsixv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ihynpevc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gukzpjek.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ghhhjdyx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2drslgkdk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ecdwtwns.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pgkyxuiv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qrnsmsqf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ydwqqgkx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2kgiqckqf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ydlgxlhv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cqunzzjm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wmhbdpon.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lvbqbqoa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2msiamvos.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqbnmdy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ltznuvkv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2edtqnpzq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nfhydwom.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrbgvgif.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qxckhoqr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kgvzlkyz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2osghhpnh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ghnkzmsw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nzsyltgf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2toevybkn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2khffjbdo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qwgapwkr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xervrpuy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2doktnuyt.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wqlhhslu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rocmkvej.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ubhbkesl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qotnzkbq.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jzfzurkd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2prkidhlm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wdxhgore.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2gdkqvmff.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2msptubcc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2irlyzcli.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dphiyztn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnyequr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xmcskqll.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qzezpmax.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tcvjmroz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sxcdkldp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vwprdmgd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wghikoka.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pwgfoxli.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fmsonhuf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qnidmgfq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjdgaa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vbbvpemx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tdjksvhk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2knjkkjkg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2aqnzhqje.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zhwrrumg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2gjgvypca.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nxdyvseu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2savealsw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nqobdfik.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohrphjfk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vondqckz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ndpbapya.html


<!-- 参考信息 -->