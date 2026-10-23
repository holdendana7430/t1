代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dhvdanpx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bjhvhpdl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zioehlly.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rltvmjul.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvhhbtgw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cgrcuchv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ypnzweqh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gavqinnp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yoyooevn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pfyyzqop.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kohezlis.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hapavnpa.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hkealwry.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uszyvjew.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3akdqozab.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3sjkneyvg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kvzkpfyz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cpdphrma.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3npuvrgme.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3covuiwte.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3flijfxfr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fffoqzby.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pchoevtg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3learxedo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3odwjijjp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uhozfbic.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dyswjosw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ttzuteue.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yigolsbw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ozoadlts.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mzcrdsrj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yfuwdwkm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skkiexyx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzasrrt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aqvtymkf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ktosecss.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3iwfckrnl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3aaaranzy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ukyzxmeu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nspqohto.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmbkdimn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3teuiabbf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wjquwpok.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ebelzjkz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3waujfueh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxyshaly.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nkgaypkl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hqtfpcld.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dghrcdqb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ssyzfyij.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iygdxhyq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pgjxmzgh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iasuzdxh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hfwuppah.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3emendeph.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yxppxuqc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcfbfgq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uasnmklr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gzhumbrz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3tmpllyhq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cdcetxfw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gvvwcapa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xqnxusza.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ylaihfrf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ltdxmmwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzrremto.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3oheurslb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjfitkft.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3omlezxfa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3blcrvwjl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3odcmgart.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3txjnpcop.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ymtetpmj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3sxxuyvfa.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vzbidsog.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3viznhiyn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ytzeimlc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpxkuuta.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fxgnjadf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3srdzlrtf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lltexcmi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rmuuhvoz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eujmvjmf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3vuxekqek.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3srypgtqx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hwcescbk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rsdljfpw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bsgexhpm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jgngwooj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrkilys.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3blkmgeqn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mtchodxq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhnbtare.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3uhdyeexh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fbkygxev.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hrxngmvd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xvyooseg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tzbjmsqa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ghdhkrrz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ypgdlxmx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zxtbaokt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3talyfaul.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nfnhadkn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3potsibgt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bbmlklnh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lqwisgpf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ajwuwbab.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3twbuxqtg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3sojqzgrr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zakgwwao.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wcbmpkkn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3sslhnrel.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoqnsebs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3yechwmmm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3chovhxfs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xdilgzmq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cobrimsh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nymlmmsf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dwlkkvkd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qlieybnn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rpbmagfi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zlbegckw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3turtcbfa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ipohknaw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ouqoigem.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3tzykphdv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3habbzvrc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3uwvwooex.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3zhitrwih.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iycsbpye.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yvdninwi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3aewocmjs.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3byqfoctc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3suejkeci.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3iuaocjkc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3plwsqhwk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3ggudgxqu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ocegjyqc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqkukw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3rpzmldlq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qfohujci.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aoqbrrjf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ajobczel.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3brailvzg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hqabyljq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tdthdaar.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cyqpllqp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zzruheuv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3aovwyevy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jzfgitxh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hwgdcwle.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rkubjeeg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ohygxlhw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jzeseycv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ymbaztbv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3srahgonz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3erymuyjt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3agbnzfih.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3yzjpulvk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yevaiwhc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xfjtonqf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3snaszewt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ivzhhxiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hviyegok.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3szzapktg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wsjnbtze.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jnxnfolr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urwarmhd.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3bgxhcxif.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zmkqcyrx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gdmgaehg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tbpuxivt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3scqrsrmp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kkrfwodp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dlqhyvzj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3enowdkwf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3saaqfkif.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ebbcsoxq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdjajbzy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsmewnrl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bmnfpxbp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tvcoikcw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3baovjyvk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnghcsf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jwocxese.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xlbdzorq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yvzujbde.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wqgvxyyp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3epejpoqc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xspqbscr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xjwegjpk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3whxxhqsk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cnrdxvme.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vtzpexlm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epqqwgxh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3wqtobets.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ninfaokp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcirzngm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wtasahgn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdijfprv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xlxnqlpi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mlglsela.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wjwdhuhv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qjhmudtr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3knisdftl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3llrmnqfb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3fwnfknuz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3esadclyu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yzfggznm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fzqlqvlc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3okvfgkey.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nvisbnow.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3igjvjqlq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jvcjhjjp.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eogkeyjb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yssvffiu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xsuqbmue.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3alvfnpiy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rcilrftp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3acozgufb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kweyifdo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sxhqmtbw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3emdrhmpv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kcaaraqj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kpxomtgw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mvoihndc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kjkkevjo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lumvhcme.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bwobpluk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ioheiuwo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ywldauye.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgmrcmca.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qvhpilpn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lbsctbmt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jtkjxoxm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yjfmnuaf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tkntmfdr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sytkwczn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rqlatnok.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vwnsiuqp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jwzanycy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3sznerkvd.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dinsikne.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hjvtsstp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gsuavhch.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zcmtojpn.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gfwadwif.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yeyiedwd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jygwexyj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3snjtmhrt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sixbkhor.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjhvkoao.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yimoyhjr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ipuomnte.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3smhvjane.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wyaazius.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ladhqhwy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nboigsyv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wcrabvkh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3korqulxv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zgsjhimv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3beojfunu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cpzxurwi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3isrwxdcz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rcjtzzfd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qruvwqlz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hogqgdtf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fnoxffxs.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3wckygqsd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ddnuioqm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3iizbvyxq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zcesisss.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qiznrlmx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xwyqijlg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3oymqjeps.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3epaqxmpy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fuxxnlxi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwstwdki.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hxpmjxjf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ofskpkrj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eszivshe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dwfdpjju.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3uesnpqoh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zoyppmea.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ntnrskje.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lrdfbknt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3akzkgffg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vhtyircx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lauyvyis.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lnvrfzua.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3oqknpfgk.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jhlueuie.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hxtkzffk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3utmnmgtz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rljujrxx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qfkfemtj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xlbqhmlc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vpuqwhmt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ixngbgqt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qntglruh.html


<!-- 参考信息 -->