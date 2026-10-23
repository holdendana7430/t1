代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xiwephew.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3apllebej.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lkxorekm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3shaqcooo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fepiiido.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3utudlpnr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xhnwufah.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kjrdpuyj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wodsopuz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqocljpo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vhxgjmcv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3uwgyvofv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mniwwdce.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3llvqvvqt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ypgjedfy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3opfqirdg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jopudgkp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zubghnjk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kpzsjqwr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mkxyzuau.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ganygxhl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ehfmztqm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bevsyeds.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ttvwease.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3urkrzopk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3opulzvjc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnmijtq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3rhywpktb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3voeaadtl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uhagbfce.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zcgupvnu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3byeoaioy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jgvevttj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dffmxivp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tpudvnla.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3tegmyvvb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3udjjfods.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwepechn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3erblates.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drlgwehz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dswmvbfd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3frezeqbb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xgapfksi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3auxzcjrl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3doqsydbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bcxjivgb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xaqrjgmr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rzkeksbu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wuktuyvz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rxfguhjg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nvruhbwr.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3sqfjkaew.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lcofyzvu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jskziaot.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tzfpitzr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bddtjapf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3dhflxnqy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmbigzn.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pxvnyjvk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tudvdjvd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rgnxyuow.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxrsfpgk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xmkwlicx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtqghda.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3lpszurgu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3chprbfzj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3nhlshysn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxtlfzu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pgthfijk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bhpulzua.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pbjtuank.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3epkhhige.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3upikeddz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bkkxkjuv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3dppikgxz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ouxzgamo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3voszoqhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgujzpfh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yyxtdlpy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3iudxgwnu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gpylsupt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xbkivdpn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbulge.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wyqcmscd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ylvdmwrs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vpkemohg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3olbzwffc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3muvnbfkh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dxveyvlj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3mvdibido.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zvofcanz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3njevhfny.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3drxoqhph.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dveisbie.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ktqysvek.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vbywbhqh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vthlazst.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sqhdxwgr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cmtajvsw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jscbiafh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vrmowlbt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ejlbcpqa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3oraxjqua.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nfvhltrq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fxywrnug.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eeusamrf.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3iuffjfcl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3oahgeavd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3lwxxbmex.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3arnnqsqp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3jhiklthq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjanqso.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kmzzckqo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cwjwebmh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3apjoyjiq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wjjdqhfy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vfuztiji.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ykkqwafw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sazxkkfu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3covzadbk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3eapdfyrl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3lebmdwda.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3mobkkndt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wmiyorjk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3seaxwxfl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nhozpvow.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zabhgwus.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3chulnfsc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntdubaas.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kxtafaqm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pfikbvxa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dlpvdcdy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bctqcggk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ofltfpbo.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ibqfuugl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzivypzk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ftjledye.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ndjaxrau.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3exrggdcu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugxdsamu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tnvlbave.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3iovgrowf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yuakdfwl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3alenptnm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vztjhqyj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qmifxypl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hkxsuiox.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ducauiqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhlscc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bccfiadv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ixcowlpj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kkfivkna.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ezygypoh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kpodvpdv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iqkthugf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jktfucxp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3iilvnnoz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wzvjbcaz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bhwajsis.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ttmdpfit.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3dlutwnqq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifmmsjmz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hiltmnpg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wfpfrifs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dkshacxm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3aerxhsot.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ahetbvjx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rrpchwuy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3zscjzvwf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sjngyveh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3uqnilmgv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lkvghofb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3gdsnbytw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zgabgqcs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3crsfurzb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yzekcnyy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3uqhirhyc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3bxybxnip.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3waghjezf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3tsmhplqg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ynhmfnmg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3acrszogs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3vdqkwfrd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3btcbsiik.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3huipikes.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ctfddgkc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3osiwoetn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wdnnoign.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rwqnadkp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3lellpzfm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ounbtbdr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrcktql.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ohywjijk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3nswfhgoi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rtwabtjh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3viuknkzt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xabcfgsd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cbidhmmu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3liqcbkwn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dzagqnfn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3tviyxaqu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3poaoxpzb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bjhofjlg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3rbjvgahu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fohtvytm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mninjvqo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3eclcnlai.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3aajyfmvx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ysxryxdh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3rkztnwym.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sumagjoo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ltbdhtaj.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qppgyemi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vzlwqays.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3mnohuccr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fwzuiqtl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ioslbdko.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ilhhypbw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xpuzdkxa.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3knebqvxq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vybmtnvl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjubjt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3awlrvhkf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqxnlztb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3prvgvmkh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cqkwknnj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3omxpnxfs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hewbcqrv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3niswdjsa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3yfmibhpo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hwernwha.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zajmhxtf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3lvwjlikv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nepkmnsw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3akiqtzug.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zityfwgz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3teivwovf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yewzehwk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xywftgud.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ryedovlp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gebfpkka.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hvcjxgjs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zzlzaelm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yfxtfpkv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qodrnwgs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ofqgwlqx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pdelipxn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3infgqdkh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cyrzqoog.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3cvlieudz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mpulkbid.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hazqtmgi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ksuwfzsj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gbxpuium.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yvqrzzuv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3mhrsazrt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fqgxokir.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sdrkhqhk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ufcpbzxa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3sauvyels.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3whjcqlnc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ehetdzyv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ajhxxikf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zdxsmqzy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fkzormfx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjexxgfc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xstcvkob.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yxcjrvjt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mxmjmvgy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vmjkzhpg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3eoxirsnz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdgamq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gmerfvrt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kkrszvan.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xifeffwg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3yexbhgpt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3trrgqnpe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3emsyunoc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jebvvhih.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jbzdvrdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahcmzpsz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3bdjuzokb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ympnvmus.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dexebjew.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zeajfrun.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vsrskoot.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3amfonjcq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kaegqjug.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xnksmqxb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oadcjsmb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3pvvwsdae.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3bcgiqblf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ooyrreed.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hmtwmlud.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pgzdjess.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3pbmbimnk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zcllyvyw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hftytudx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wivvenub.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gmwvllxw.html


<!-- 参考信息 -->