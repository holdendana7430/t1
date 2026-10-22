代发 wailian999

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sbfhurbb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aiybsdsu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zwbckxuz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wahuemzl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2thvtnxmo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2sdaeubpb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zmkqblet.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zxvgesez.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yraeifcd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lkxngavz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvhbipxk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2dmzknxdv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rvsdtlsk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tdvrvppj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lhgmabis.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ygbmvtpl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrzgqrkn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mpwvvocv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vlxuymdk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iwwvjfkl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2onqzjpts.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2leoakwea.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewrmpivb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cvapxzfe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hbhsqyli.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dhdkosih.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ngtyukdx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qeztmynw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tfnagjif.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbdhfgqj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vazhabde.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxbfpsq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jqylsulh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zolvzgxt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kbgaysxv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nabimkua.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ennuzfye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rkxgflbi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xjnpspiy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zhlohdjp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2tkjyfhrf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bouetamj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bprqggqz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2wytcuzzy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sjcrzufw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2isaklhda.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vzlpbqad.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2annozxyz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yothzjcz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aiixsbgm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezrkxqgu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aqguzens.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2luuoljly.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pqmctwda.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2espvbdgl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pdullwxm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wbezogrf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2byrxffdb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2icsuunpe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zahnsyat.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbyisow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srqhvfca.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hslduras.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngxlpxvn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ljgptzmp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jmacwcan.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qzafvqid.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npsvpmex.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bdhaoklw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ihiwuizu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ryomrlkb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vicaqvrq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2masoqlip.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hksgtlze.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zrsrlmsp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2swoonejz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ypfpkmjk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2aldbzplm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2utzetqjt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hvvqjhbe.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2thuwipbw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2agtbqoxf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2atgoourv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2mpdbelre.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nfeswtfy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2psggrfuo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vfazghka.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbppmbvu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2izhsxnbq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdsyiso.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wooiaiqv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dykhecte.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vrebjpwx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ncfrcfrj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ehjunuqh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2slbpzpkd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2worqviah.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nazrnldw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2odnidclm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2sxgpjfjv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sscupakq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqpbwuw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jouuowno.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2pimuqtxu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uhfnopfp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qfmluvkg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2okocbhma.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lozhgcnv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2qwrpezhw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2sfyixtcs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2reohmzyu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2szkfoddi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bbmebdip.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fndlcjup.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nbqdwzih.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhrjrwj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yfbfbdof.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zjrwpghj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xxbppmas.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2elgbddox.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fcvikgid.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gbnetbmj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nvkvhteo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2joqcbuaf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ldzmksay.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2omqnirdr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wedjsjck.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cumjhznz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rrspnbco.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yjejrrxt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2phetfptf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ssfskkbu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2nobdqcwt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2flzznhmo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2eugwclhj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kyqrwhmn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2nhsszbds.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mknqszig.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nceytcje.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2euivuuby.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uskgswmd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2idxccxwx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cfntjaap.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfdphjw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xurjmlii.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ottnwlld.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2zhtdzjmh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ggvwoerw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ocorlvei.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bqaoxjgy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzthtigi.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zwutiseg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qyvssdxf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jgzpycmj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2azfezgiq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2uewfirfg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhhjmkxr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sguuontf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2bxmnspmi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zldwbmyp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ufriczri.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ylwisbcx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2inrxrauc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hikkmkqc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2szeoeckq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2barsfowp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfsqcrih.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ulvicamr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ezurewzj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2aontudam.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2jetvgadv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vbpylmow.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2clhtplve.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gtptfhgj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zyyyemuc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oauqcmyw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jravluzl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwcaydli.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2toogbrng.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jyqdxtip.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2obgsvpxv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2azsccnsr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2herwuklv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2cxrnvibk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2notfnkka.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qixidacj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tzfvzxtx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2jdkytmpz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zageblwx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cpjstkss.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bvarjwle.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vxawhrmk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sgfhgwit.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2anlwjslh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wpupkcjl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dcmernln.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2vrylskkv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2zvxkcucn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2yztcmmhv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2btavafdn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xgcxfyer.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wsqovjmw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uaayvoyf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2llnlsoxk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2okxaqakt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2upfqmbfh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bucxbhej.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cwgagjae.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nwqbpfdd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rpwaruvt.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2malllphc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2uakvwbgy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fzfzslhr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2txrzwihl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zdhsyghm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2stwgxvsl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpzfmn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vfeaxlti.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2psxznjhp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2svlvnekd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cazvkwdx.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjsgtz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hxqyoinv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2eegvorgb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xscheajq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2niledgnl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xgggqigs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2baavjqpx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gqrelssx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kppjigig.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mwxvcnib.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xdbpjbvy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ntphisrr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mjifuuhm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pgyebruj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cevtbjeb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ulcefskh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2drwltgtr.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ztpiwzwt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2nunbclcf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fazwdjsq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kekrhrag.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2gugfwkdj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdhmvnpr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2smrmmgen.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2wlsootcg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kaebrudu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdiysmfa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yuwkzjrh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lwdtvacp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxlmolsi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rgoitsnq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iznvekzg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2naetjyrb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vgzjyinv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kiyvhedx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zzdcemfq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ymqjngay.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ypjzeruz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ohgxbdft.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qgfmakzm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2uabrgyis.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2jzzjkmpy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ovlrtind.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2yvebtylb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wvqnixnk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kyyonynh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2guqvclqw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wvnanrwn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zwwlwdsn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2tbyzmgve.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pmwhzluk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oqrosddr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lsrosefx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wjcntutc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2zdkyyvxj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fyldiccw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2erjpvotv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xvyzigsa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2eedyqcda.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgmptrjh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dulgkseh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tkhcfrye.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2apdugevp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2csierkfn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2thaywqss.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lnnswdlh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2trfosuvs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kavrmigx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ydzremid.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2snzrdvsu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hybkccfm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cbbjsxjp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2smdqzpme.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lmgcrqlz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2octkhchy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uxwqvofr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nqtcvuuu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wlzwepaf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qaywwmjr.html


<!-- 参考信息 -->