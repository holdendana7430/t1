代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fmsqehdh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3voczspyf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dqfcszzy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcpolji.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fpsaatyk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ywyxrhsx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmgwdebh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixafkgjd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ggkoxult.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ywxuwozn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3iesmmakd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xkipcvsq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cpnsrddn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tcsbcuht.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zctarpnb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wfrgfnjc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tmxgomjp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nrdcwntv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hwddxlai.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rhuxcjqp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3msfbwjdi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ikyznnvr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3neqsnnlb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pjccvygf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmwxddsj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iqihzqfk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3icxxewbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pkglsgbz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oznqzrvd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mhjfkhic.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ywrkamxu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qtntspfj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fiqlkdne.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bofhflzu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dlenspml.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wfjwizaa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3eesirhkk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jwqomzle.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nnftjevo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3apgodprn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zzcbufgq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xcxfrobp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lkhsovsv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gtmfvkkn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwtyossx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fjrlqpah.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkwntakl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lvyzzvph.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pqutplva.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ooupuloq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xpjkcsey.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ocadmafj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awheflil.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aferaakl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mfdqdgop.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3oxsxurwt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oadhelll.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lmdubfem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wsmkgdke.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3uiitsunf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gyldkfhp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pgneebio.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fmnyupae.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rgqquiph.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ookyzeeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dysksxhh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wpfcgiqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cckpklxo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ltyasqmc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3sincwion.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zjjrbomk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ychhhbpt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xlnzsskv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nrnfygke.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ziesxqas.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fvryxebz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zmewayqp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tpmvckcr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gyoapglo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zwcqasnf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wzxqrhhs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3faaicfmc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hfvrwneo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qzshuhcp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xkzzgsoa.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cucfhqal.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qknpodsa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3khwnrvxb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ztsbfyqj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3smqrctrh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3diepwxth.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ifoghzzu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cubzvgua.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hhqzxtll.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3cbfkugtt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gvmkqsix.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pcaynypb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cekmsvwy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lqismbdu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fxbpvigc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vnwkjjil.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxdeyks.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qmkwdvix.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ewuulgah.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tuildjqj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyewueat.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3grslgvpk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vdxfgnwl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3peeripfd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qcheuyzg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ahvqweva.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iywoefng.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3iytlhxps.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wwtwvvzw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jhbyhppt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yxplsnee.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yxsjjawx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yvsxjzfj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rcxutbwt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ypqenydo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3vdykhnbi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wwzrywgx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3czuvbvuv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qaqdadtp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gujqidlr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3flcbndjy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3owtfhcjv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3waipbirc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ryzdquqd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lznsapwt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bvkumkpy.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iosvmnuy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qjtbwzln.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3blgydjnv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qwiupwxd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3aeahdyfh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3iplusuea.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbpgftt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qdugicdn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ereehysr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kbhsaxbx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hbiqlsax.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3niaduvfw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ksuqddtf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lmmxdhey.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cislkvpv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cjsfwvas.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uhogdbme.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hpauopvk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ztkvcmzd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3oomkxokm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vnppdqdy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vdsnsoaw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hnraojmq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpwrjcpz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yxvnwhou.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3asmqdcix.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pdsrsbtr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3cmpprdbs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vssnlpcl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukxwiimr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qqohyeqg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lxhdxnxl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cswyubud.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rwavvktb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kpmsgaaz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3bcfglgjz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bbskjywy.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yogwuqnh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mlorpkem.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pcotdyoj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cdylbgdw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xyafeqju.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3lvtizyxe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ctfzssfe.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3iarzvtes.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3czpdnvrv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gzblozsx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yhqlodcz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jocwzfig.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3muybsgwi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkiwyaej.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rqgjqrtd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wijbzgni.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nyursggr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hoqtetjw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kgnatdlr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kpkssfkx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3omhxsuef.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hywycofg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cxauenal.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qnhrzcdb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gvkvutrn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wnwomqcq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bfbzndjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sgfiuimf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3lpcnwyyn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qnbeqijp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eekxtrgk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qqdbdtri.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jzymrvef.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vtfjmmgo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tcedhouj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gtcciknj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3vbzpbmtf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mozusuys.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3geeqngmr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ilojodrn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3biuoyvzc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvahgc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3liiyavqz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3sofavdim.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hzyjtqwr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3upqsgdww.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qffbvmxb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ttzuesyu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qispverw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ygiwyfdh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3giagaxwe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zflwxyys.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lgoenvmi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3wagptcxw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3famtaoat.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3oskqjdlc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vypowugr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tdtyiwer.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3skppzjyf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3qpkwmcni.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3rcdsidxh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lcraxzzb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ofmcazje.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3cblgcuxa.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jwcgfjvm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ubkkoseo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hoburogm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3aphoozkt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3chdescse.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rcgllzwq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3fvrtvtym.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3kwbrutib.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gruymsos.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3thzmnezg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qwxjpqrd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gnymkgll.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zhrxaznf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vyyiojxd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hclnoqov.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hvadolkz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dakqvqld.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qeodtlok.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3islorzji.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dkfrtshf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vlpaujmn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wniahkho.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdofyrom.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ktdlwbzv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3czckzese.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hkcstvns.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3fblkaxmw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdooyvvp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gvynzyyx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wagvujam.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xpmczyrt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ltprnvui.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bwpbukea.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3eoshmqfy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3eribkdnw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3voojojwj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3emhhvkxe.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hovdjtgl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gmfpyvod.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3btetfiov.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qrefndui.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3esiawgqs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3esgxsyiy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gjasoede.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vrqmnndg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jinrieci.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3espqweuu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fhuvcibz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hhyvxppt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3esdarvud.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pfponpmj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qspbwdxf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bbrqbyuu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3neezeqmw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3irrsjiyv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cgwmshos.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3aldayhse.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cqczraqu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yfccbcmv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vdfwkvmu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pryuegrw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iobbrqug.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmbjrrid.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zfxzkjoo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dyzddoak.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qvsrgaye.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tgattdmj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ujtsqeam.html


<!-- 参考信息 -->