代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hbkasgas.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ilofoagp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ollhzgdm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vcrnecet.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oeeoggpj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ummqdlxn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dntjnmxg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uagyzvxe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zolnmhxx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3kcfirqus.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ctylrxtj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtqsgenw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3coxcxxak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovaupuwe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fubepylg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lnekeluq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3accdkbnn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3onabdkhw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhtqnuuj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3psaimpri.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ancgwscr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vfkaodbq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ghdusidz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3eaghboax.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mbsrplee.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ttrrslnf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ubmfbvfa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bauzhezp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xpmtpvxj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrhzpu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xrqwhhbs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lghatdob.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3svjjfndl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ypheddos.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jpxkipou.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3piggtvnh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bjrzigal.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajiyujql.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3clovoaam.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3mtjhohad.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ujpttgvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdonzgab.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzupcpqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aumyugxx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hkxwnvfc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hztbyrbp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kambtisv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3caegyhnl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3roloprgr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zfksmewq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3lzvhaujs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qanfagzq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jcuxncan.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3evckxtln.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gysdwyfj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3pgeyjjib.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ddusduyb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dgltprua.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tzlubxqc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mxizltwt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mizmvbpp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3mocuvhqk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ttukfgwh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yideovnf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3crojxmtl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gfcmzzqe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ihepvwjf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhgztcs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cutoktkf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rhstewjb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vpxmwxpn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dednukov.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yjtebbmo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dtcwrmym.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3nheatwew.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mhchqnng.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lowgdcfp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3aomqlfqo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jstuacma.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cgfmbobm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3eicytcob.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tgqwqsbc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yjmoicjm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vlnppqrm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tpiguzep.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wlilatok.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vfqdtfvk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tfmiuayt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdxzfxol.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3dmsulcip.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gvyukszq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3erximgxv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jqxxhjsm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnnader.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vmuntlrg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tiwhgvle.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3eiezgjdi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hpjwgcuq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hgeummic.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vdutzvka.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ttmfrlpu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vpgyltno.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jxrcrdxv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vduvydtm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xpztwtst.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3sfvtpssx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eqofqcui.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qqtfesbg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3kxsmvxgk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3refbwjex.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fdjylitg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3nyknihmv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bmsgsxfp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3helxojmj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3spbfjlor.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uytfjutg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nohdkxzu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lmkniwcm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3yaatkexh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xpmvtghm.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ceivacsf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3yxbywzpx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3znsymtas.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3keppbqjz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jhpjtnyc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nxmbgpwf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tsccqfvj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cjhmhlzy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3luscowhw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jmgeemlf.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3urkxgoqu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dimrvuiy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3djvcayqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etetzzsg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kzepxjpu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdwinq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3qarwvsya.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3olrcalsr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xkiormng.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvzmxnt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fvujiccs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yevfrohb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3rfrvbjfi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsqdscwu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ijhzcqbv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tcqqgznf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sfnzrgqd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wowetyog.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bydbvxpv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fylcwxuv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pvioxqvj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qvotnaoy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wvmdmhhl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3htfxgtqg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfdldslq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkfxeah.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mhnnwtjr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ufosbzga.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bkggvubg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sntitifa.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qyzepepl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eauhoyxt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tzycrvso.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kkqlotci.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mcavrnsf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oohgobxe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3odzbirmz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gndlrukm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gscguajy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3iprwnzil.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lmmzgqat.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kywxxwwo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xplvzbxr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mpyqnsgn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jvtdhibe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwuwsyck.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3knxpojty.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wovvcphf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3yvwdmvtv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3eumhkxuj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zswoswtr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gshzoseh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wierecze.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ejcufhtz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zucnirte.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hnmwtmpn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gnypisul.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yepwunfa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fsajwsie.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzynqny.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nwavxxnb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hdhmjobv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jcamulsl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wctfjeyo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vfkcxzlt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nbfnloid.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yzmngdaq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3hhistvxj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hjnukjrt.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gvvfwycl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3zqzwahdb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cjzrdntc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wbfevrdg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wfkojysx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dpxibwmh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wfutzmis.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3fvayvpie.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cighmmap.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xrgnzpqz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iqziaksj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xincixpr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ccpwctnb.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jtysypwh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3nibntegf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hipedtaq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fxdgtxso.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3nnglxgzg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3yhxlltzy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rmesesyv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pxwsbzal.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3xrjkdhpf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3saivuuga.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3npdvxbsi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hkwtpdmz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gyqfzvlf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ffszniuh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mgamwjlk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbthawzg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3frmtesww.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3oclnhnow.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gghhcsmr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wisquesp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tzrymnng.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vcidttnz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ormeqgxw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pzyuwowz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zuefcbtd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cktkxrdq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3geprweqf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3yietmtuh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wwcnmigi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3tncaqpll.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bvhdgxct.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3prxszfbv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3itwmkmfz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3smqfourc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3evaumkvt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vfrylvtf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3earnafzd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3uekxjqwf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3chjyueom.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jfizraid.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3rmvznsin.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ockyxpef.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mhdjicqb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pupxgtde.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rrahotkm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lqtjyqld.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gnhcjsuu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3arhnrkpi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sprnhezj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lxdbxfok.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xalhttnr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cdsebwuh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nzrlpqvl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hskcifaq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qmprwejr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ucpczwjq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ylbxqubd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bsqoonbi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zgeqtjjd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rehcvsrj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hserpdbf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wudeuceg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xqplkiik.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntnreutw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3symdnwhh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3sywfrmvj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3yknzgcpw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3bckjpeoc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mrrmcowp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3csuarjyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mspgksnp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rqjfybxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdnhnmjq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xeagcbve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxxcmiqr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3aofiglln.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vnkktknq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vnwbnebs.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kjvertlf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xwbsgxzl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tgdabjgf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3faaaualp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kbfbbhjm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xosqcdxu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kjwsrjtf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aibseodo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qtxhgasc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rchicagc.html


<!-- 参考信息 -->