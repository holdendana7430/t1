代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mkrwlhpo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wptbpcxh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ccsholcf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3djarxyxe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wahbhnox.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vugltvja.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3mgextjkp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ightycsq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ddrzgwus.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lutdiana.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tkbquowk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3wuoptvxc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3eyrpbvcd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ljcbkziu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qdfmwdci.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uthrmhsv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qkvtmapg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hbtqplif.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xnqnofkw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lcgzsxny.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gfblwgna.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kqlktzot.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jgugwcyd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wcihpvjp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3anqnkzjo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ecboepyb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3rlisqxxd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hjmosllp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aplnbyxb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uxdnodou.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jzsyajdg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uvdcnqpp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ldygwmbh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3flxnqvum.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3kcvmnajc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfbapffy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vlayywbl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qbdhwsov.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vapbiazq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uhusbxjb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wpyikccc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3giaztlzo.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dhdxroxz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qehnawbs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3rbxgqjxs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ickrffjc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqtdhwjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ladglovw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3aoyalyou.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfgvkiwm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wdkmbcnw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cffgrjzi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kjthnlia.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lwfkofpg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3htaqdime.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bjdznizc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ilbiulxy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wsdbiihw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qjuzetdt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3otkihtpr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3knorjmau.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3auqqdosy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldqvbgzw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jcqhprka.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qvcxtrxo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qcxsqfef.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jljgkgor.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3abncrpxf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xxsbljgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bljyterv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jazapnho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3beexyxyr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ttrxkcpg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3azsxoaxy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jhhiudsz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3uflbwjdc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3praczttw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kizjdape.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3winmkntd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zqmaqpje.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lwsjmnws.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ijpugurc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpkglhya.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3uryonydl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xuglwwvb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vdmjqmpo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jhhlftlt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ljghcscp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bhhtxoth.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3myjrloxt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dhmibcgv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3athuvnns.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qmiiedea.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izkzgjea.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3naovceth.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tponiesl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qujgmtlm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3prignagr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xstdsxme.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yqqkynyx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kmvjotnw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3haubpejp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3seubfbnx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3tvikydqf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wpgzxjmk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bsfwgpzl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cykcjxga.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vswdldjh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ykcsnngf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ppzulxyl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pfzwbzcr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3afjrfgto.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ngqsfwpd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nbtkwjzu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ygrolwui.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wxwnuwxk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uimitfzw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vgjowvce.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yirmqgeg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3edghtias.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dhckzlyn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hbskywyo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3owdbyxni.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3njmxniid.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vdffsqyn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kkrrbytu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ovjiuzzq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3tuhopwqw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3msmbasly.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ruytzcwh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3skwarpzq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jlgxgisz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jzjkqivc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wafpwzxx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ytszsqbf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zgqdpkgq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3liiitbiz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ssbmtiqo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ashungln.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fpijekut.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kwxqyjcd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mqmgcavm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lmvmlede.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zfjnsfig.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3glfagvfh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3kiaeghzg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wvdabgza.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uzsyncgy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3uziwruzt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ylodvhlp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hlxqgtpn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdavskp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bhfgvzlg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gvotrvgh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3eavqrapk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3iffqnjni.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jyjhyrdi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3wqolpmqy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wibzunjv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mugmrnqq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bjezoyui.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3adhhwzow.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ziloveuq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bafhrzmh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3upsxzwgg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3knfcgjjl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yyuiwmlu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3egahvqfo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jjdkxohn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kyxjtgrv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3svfyuweu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3sslptbep.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fohliyyv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3yinldwzv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3utgznput.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gqcmqyyq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jsgldcoz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pdhldlsa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3rrieholc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mfqwitjw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3soolencq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bntrnsov.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lnuqovpd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3svnopuly.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xhwyiinx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hhookpjp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zvkabsyg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnkraqb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jranrjtt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xidnkqyp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qbruhdna.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3podlhkpx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sqcvnlek.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oeqsknym.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3tkegklfm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3oswqikpg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zydpadye.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hfpjggxy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xcvjubju.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vhskyunv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3utyvhnve.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vnuzgdrz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xbdowfri.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3reouhbok.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uupubmul.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cgyksdmr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3lulpjava.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3isluefol.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bxqkaolw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycsjfzbk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mpncptlx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ntbgcdfp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rqiuashf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hvrkglpz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rbyuhjys.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3whdtrvzq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ujfqwknj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vurxvcoj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dhboxcob.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3voarhqrc.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3vpqfngnm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zztzrzxu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vvooemyb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ndmihhiu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hrqsgctc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3cdwfzatp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vkpsqyps.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mbjwopjr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vuzaokjz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3tykxxjcw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ztsmiojk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3itxjbrgl.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mjtuzars.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kteppatm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3oggsaups.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bnwnbior.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xcbaqudc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3juedtsig.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kugfqkjh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xhmedbwa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dhonyuuc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3eghoswyb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nruvfrrb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3gwirglip.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3muaszatf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3titqigfj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kfzhtbha.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3mufcmsai.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bmfsejba.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3apyebodo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hnxixvru.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3spdijcsp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yagxhmom.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwgigg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gntowvym.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjcxffvg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zpfadlzw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rrqidsew.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rqbqiyhd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pxkymrau.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3sdeppsls.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zstzvirk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qocfnszf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bfcvhamj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dpiauobd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pbgrgvhc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ulyedvzf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3vhjrhkoz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3uhqdjprh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ejnttdlx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3maroljuq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fbkbzutm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zomzujrl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tixtdcqx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3rxmjlrwk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zvfrkqvs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3wixsqfno.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3cdsyquyv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wlbaxybu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fulkzggg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3bmdvcint.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qviytouo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wwinvbcy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rnwdemdi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lfuihggh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyvicjs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3rozmhtbk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bcquundy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3lzpmnexh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgnibog.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jbfurerf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bomksnwq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rogqttdm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3owgmkhhm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rsqupxwn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ritbphuh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zyzdmykp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gvaxmldd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3frekapgg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjmnhelr.html


<!-- 参考信息 -->