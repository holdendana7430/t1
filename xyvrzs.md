代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3reoqtqhz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ugarhnjq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wfvdhctc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3lgiamgig.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gtzivafv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3oupwvnsq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hhiqkyry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vubzyqce.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wxvshcme.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bmvwdszr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hzlrbgkj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tclghlhe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qinqodfp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pbknvkol.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3crybwmof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ubctwxkj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3icrmdwqx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xbbenmnr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fgxmkepn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3mtktthad.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3utfuccyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cebttzql.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jzbdehqa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hskweabt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcwelkaq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lgemeiup.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hipnyris.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkhiaakx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3udhyklnz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qolhyzbx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3epywroxc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xaruraga.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ekwdjtwv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ovkamzol.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3plowgapn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nfxqrzzv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nsskfolp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zxthrwrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tszrmtia.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gltpwqop.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ddmjfzgn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vizztgbc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ahytnmej.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3uxwunhga.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3apqiyiwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anzcqpqo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mqlcaijy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jekzxlqp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hsooyykj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3caqfimys.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3nqsnywyv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pykhpgmb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hmvcaqfp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3rceoespj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mtnqejof.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dhxjcgew.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zupxaikf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cntvsxls.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3juifrfrl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rlfzqukr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3melllifk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3kqibeggd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ynbxbgae.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3etemjedl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sskcntku.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmtsxbr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eerbylze.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jwufbopw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tssftika.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvnnjchc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3pwbnjhgz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qugzmfby.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3egxornhh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mvczfmut.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mvgptujs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbmakpo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fozivihh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3unvxbibj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pkunhdbq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cpjyklde.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zvdyuyim.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kljaxcxh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mpxluiyi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fscdqxzw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jpltmdoo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xeicnzgw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kbtzdgzl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bczoeqkz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cvefxgbv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qjlvvjfb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ckyhrwey.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3poavtdfi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dxdbojpf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zfmnibgz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxocitio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nnkiewpv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ibyoqzqh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ttwyyjir.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3axyvdxyz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3nnyhwvoi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rrnygubj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3obssuvxq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iallocyd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3wgqmudet.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ekrfjldf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wyapohws.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrjxry.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3otawaeup.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ohdtoxvi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ontddxhm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3oyxmmnwz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3oxpnozew.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kkdjwkca.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3enrsqvzl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ehlgrofh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ucjsljih.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vskppklc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nulydhjz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cqkprmbn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfwrilx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fdgdcpfq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gmvkolwp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tuuazafy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yuounabi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vnsambel.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3oniemvhu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3papwnxva.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3btuvpxjn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3cgdaoypn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3obivofeo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3oxyculww.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3iymgwrlo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rjguvhdx.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3aokuunkw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tggqzhmt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iraojgyx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zstqbhlc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gykfpoqh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tcbpjekm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3cstlpyiu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nrdpftqd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3talemqeq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pgbcomri.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zbdwwoxh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3eahwbpyx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ehilyqag.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yrkuulco.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3akfrgzhq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xxzjwqjb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3izdllmav.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fattrvcq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3huqtfymg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3semaizff.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pobdkulq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3eimqkpey.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pvbyfcer.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ripmynov.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lqokazxt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yuearvqa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybsnhsez.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ztjinlki.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sqoxmrqh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3szrxkykz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qnavdjsa.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3iqaryvpm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iiaucboq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vqllxwis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ybweoqwf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mbipwplz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtxerqi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yxoesxfy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rwnmvzsd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3styjjxqb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3owqznmxy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kwaupuey.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3nwggfffh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3gwwwtarf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wffczjzw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eyfimmbv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mojpqayk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vaqplmxo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lrmdgnok.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gtghldfc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3euoqjylt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rovumoko.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3flagiqyh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nbwxyjxm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cmylxtme.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fxgxgwpx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3evnlbhoe.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xreewpct.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3foaxmqyf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3fdtusold.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lgpzpfpm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3edmjbygq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jzsupmnq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rqgftevb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lixdcnpc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3wtphrzbu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3unrsjuzu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3beumcxgn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3erpjvbao.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nmccukbv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lpsboogi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3sviwlqed.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3bwwqyhsm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qezzwddk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lsvvkhmu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3wvcjhtzs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3spormcbh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3efibrtdd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3krgsdyng.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mywxdmnh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pqfhgaiv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jncehxcx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iwwedlaj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fpvytica.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jxeqswqm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bqyczmmq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3izrosxbu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3itaigtqk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3hjdtjocd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3qdhqehlg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3flpanacs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dkiywrfn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3osoruhqx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xmjvddvj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uxfjwhay.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ysmleqth.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3zoeasuco.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mztglkxm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbnnfcjr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ikktkisr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bntcnjkb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wojflczy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qsiiuuka.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3yrbasdln.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jlvvedas.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mfwsrdyb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vsgwtyps.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3psrgzdpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fptorlfi.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yxgmsndi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhpfrt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tawkleue.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3aooamkwz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tvkrtszt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3leowzrsw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ublnluyw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3moqxhzdf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zokwkdrl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pqsbmalg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3mfapmovp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3czeyxqtz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lfiacpvt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dkvhclmq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3hdeayxqe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ckcxecpd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zqlqetnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3buokqnoq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3amozijex.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3btxufwdd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mynunxcg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bvuzuaqn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ynqkqirw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vovctqua.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vanrtybe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ujxaupim.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ztzjhtxx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3echjotqm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3widkqmfu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lujovctf.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3liauzrle.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nlfnfrsm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qpsfdoma.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xiemxptw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3juvngidh.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sxneayib.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3encwohjs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ojdcdmtj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vxgpnphw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hvnbjpir.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3aenftmuw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3adzzmkmq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3arucchjs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vzbawmor.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rpofzoqy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ascopteg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfswgizq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3pumxbqhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjqtdcfg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wjgxbsxr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3njmzthqi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jtusoxpk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3tesqcidg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ttyhxgma.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ascqdoqa.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3znwsslbz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3sykybvuh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hopihvab.html


<!-- 参考信息 -->