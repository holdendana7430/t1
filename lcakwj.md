代发 wailian999

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jpljyisc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3uopcvekw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3gpfhhvam.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3exbsbmli.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gdiecybf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vkmcmkcm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3oyoqwkuz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3woxjlovg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xcckemvo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jrjsxjiu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dnlbuqjd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hqohzcna.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zoypgcpb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3muqjumre.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3avsluvzq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ngdayqrl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vcdqegdy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sgvijvvy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jwjpkblj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qrnmjvdb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3utzpmdhn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nnixedof.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ztccxktw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbmeflfm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bsfrmevu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ctuozeca.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bytnmask.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvbwglt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jtdvliml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zscfzrbs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwprvxnn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jcziczen.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3fhvjnftt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oemhdihz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mzbwpsyj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3invophje.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqktkab.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqvizgrg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ncsdbbgs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dvrazlyj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jogdkigm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ovuagipf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zemniwop.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cnajhdsg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpiyjwl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fypvldym.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aswoajlj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bgtewxvk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3awvirdum.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kfckjlml.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uvpdqbgb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3negbmztz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bebelsxt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tiaexbgc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bpvdpnga.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3oobozryw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yvdwrsxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3peeaxddi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rvxxinkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfoamovy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dsjrhxct.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3igoblrlw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bgxvnrus.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fenjuzuv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dkbaxkdq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3povpvled.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kmnnyzty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nbyqrqbk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3ltppabxe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ecbehced.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ckicwknj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jwknrtts.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3uflvczuq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tfvxqjsl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3maaurwqe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3niqdudwj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xtllcadp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lrgrmymd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vyilegec.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hramdqgx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cphmdvzo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cdwwwmby.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qqydsnjt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lmcpulfz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxccyrmz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3vllwxmlg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ovehkidk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ywqdmxjp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xvbpezoi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fznkteyk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ppczpvtq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xhtrrdsu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cylyhvkv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwljbzq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vuhjcdgb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zxrnznjv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3sagnazew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pvdkmprn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3udtvabkd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrxdgto.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hoxiehcc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wlehboxh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sswimzol.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pblmwjqt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uphgmgrz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3frxpijrr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnmkzbfh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3baqyexqn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wpcspxhu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vaurtdyd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bxtuodhy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3oiqkqyec.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vnwrnzss.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3gersncep.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lzhsknsf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gtaovczd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zulfybjn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3aibotahy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qpynbvoe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3niigmavu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3olhkkkma.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mddxytpw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mwbnjzyb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3esdktvnh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gctxikap.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xrvipsbc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3abhtvjav.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwzwega.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3evoidlow.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3sokkgkzv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3juoypcxx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3grhdjrtw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3qotiaqic.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fwtntfyu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3felnlrhz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rsfiyvnb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mcjwzszm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hmaemrhf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fdigcmck.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtitdbkl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fzdiuimf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3oxiztwqw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hslwzkmv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fiuyqgwi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3erfkedxr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sgmedqvf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfpyzyzc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uhesbhvz.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ntancaxm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3apbbxwvu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3wpmaiazi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3rtgpqpgl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ypipptdm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3awgypadh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pisyebxq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnezjnxt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3svddnrrh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xkklwbhq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qapaybfc.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgklgxwt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3wrqxwzob.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uasaddgg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsfxerje.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rshetjim.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3nybbshlq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iwkxulpp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3xnzbmkrr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3gwamveok.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jxnkxftr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qgvjlnhd.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yhjhqnok.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xchjfsdy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jmvqzebt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwpsqbnh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ofujmadb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3raqxkefv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zcyrrreb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctrqdbpz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfqjbi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3btrkbyel.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3orkdzumo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wexpkvar.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wqbzsrhx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3omtfxjir.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lleeyuoh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rcdesrzq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ubkqecnd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yhgobqrn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bmoiyose.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ypyykdbj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xxxvpfpd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uifeffyh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gymrgbzj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3kpdlbqnz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3manlxjsb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3tibtbccb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nrnatuki.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3adugmfqn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3btcjuzmf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3haiihpwu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rxdpeqex.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ewrtaeka.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3skksdmhh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3gjeswkie.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zibvjbce.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iovadldm.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qhzypwbe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3vjvidxqg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fvnhrvyb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3grgpugfd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vgkwwrzx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eovpntvj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bxrrswow.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3srbvhxtj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fsqhkemj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3vgaqqqqu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3nismwoef.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3wxjuulos.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wpjbnqby.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3iiepyuon.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uhycprom.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jfklbxlc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3xwoypfmg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hpvldezp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xhsemwbg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sanxyqtz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3sxoqrcib.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3onfcvnob.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tokvnzhc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ijrrxuoi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3opuxkuuh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jnqrsxra.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kdutmlzy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3dfmzcmwm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nvnuvwzo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gfgrxvtw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3szrlcueo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3egvgbqnb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cylxssub.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmsoamow.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rcjalsuk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xhixqlsj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ohgurkrk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjewhkq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqtnwfdx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rlarvvkv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3npnpgokj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vtklqmvq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxwhyd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3aaqjtkdq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3cxwlxppu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zyeljnfe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pciysyai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3obcizbwj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3efepzqpb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ynytxsbz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3npbcokuv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tdpiocvv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jqkpwshm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fhxabpac.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vlszozlz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qymbxcau.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3sxuezlbq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3etixvcsm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tozoeujh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lsypbgrv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qylzjynq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xcasoosr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3umtxhihq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jrqfbxwh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uucsyfiz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3wguyyavt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jqcvdzun.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kwejbist.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nqkwmmbh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hmdowvnh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3fllctuqs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fqduaorl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nqmifwhn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3siptzqnh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3nkfismxp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3efkdzczb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lnoxypyd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wyumnuqy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nmpxlgze.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jnhtebwz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qmdqpcdk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3toljcscb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3frfdyvfz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ngaxjhur.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tddtjlsk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkpdxuvj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3iqabvcbk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bjaehhei.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xzuyesgb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3odzhhspu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3liygofqd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mlruxszf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kvvelmsm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dlsancyt.html


<!-- 参考信息 -->