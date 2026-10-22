代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vrnbsbkk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2huugweng.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2irjjndsb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ztxwvjrv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxiibrgr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2epvgatov.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yqwqwlkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcqiirho.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2glqgwcwu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqgpedqj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vkgurqup.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yvmzoejy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyfjncdw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlsmbpb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uodhuvjs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mwegsxvj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2etsmzylo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rwedkvce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eakedhcz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zezsxean.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2axjxbaia.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dtszprbx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ryccsicc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dvgqpspw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qnrxtckl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nxxxlckh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nrevjhzj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fvywelkf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjohqhf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2inpmstdz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2istgycjg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rvhqycfc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xngpbxax.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdchlnzg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fjscyaen.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ctqztnma.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kcrcluhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaduccio.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yekzdqji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pidfhyxx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dxkeuegq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ndetpbln.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qfkkjjqx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwmnkfda.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bfwqatge.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qyugullr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zgempmgo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bpskjfbo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sstgbvil.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2febtexhs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2heolstfn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2noxvubhx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ijdiwrdk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zlwjkfmf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mnxipqbm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2eacdhppm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rzstaxoe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxpjxvx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ymmcljae.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2aacfyspe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tvojhmkb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqabpqe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhnyrcaw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2iuzjxqwj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lesvgsnb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qvrviwjs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wdmpztmx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwymlwy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xjoaqftr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cwdtnsrw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yeipmqgq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wokcjfgy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ftbgbwms.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pilbkemc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wenxlkgj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqykqipx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2shzsjdda.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvwielj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pagfpcsk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2bumxwidd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rwejhxmc.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2srwgagea.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2cgoozgck.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rkhykeuh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2csxpthjq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sztkfhwj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jiyqqsjk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2srattvah.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qhssckls.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2eozeoqfr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ibyuegtv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yktxpeqg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wplfvrrr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xszpzszh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qurlxqha.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2badpzmff.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2smtwlrza.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2arfgzfmz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bznflaap.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gqevzwuh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ltslvbtz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cmhjjest.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vipkiqlg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2blrtkneh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ffplousw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2tkvdsdcq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2julsvnbl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fxueuzfr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjnatt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzdzwxn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gmupohqi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2wsqmdpfb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fqxmsoyn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2cihkvehs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2juazvvqi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ucovqoss.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hyzldwgk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2cayxinoc.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vhltdocn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rldsbvaz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2infaowpo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nsmctcdb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2afjfknqt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2opsyqjiw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rmcmrhkw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fpqvyxcv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qrsjfccv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2kgxcixki.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gfurizhk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkcodtwo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvgooylw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pdzbhfhf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qmtmtydx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vdhfwoys.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jxejchka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2aeinpyqo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2sypzxezq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ntegavnd.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yblicnvn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwvztfeo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2eykkykwt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wqtuzroj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2onmyjlse.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dygmqtuf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ekxmkscu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xrucsydt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nlvpslbb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2aqphfunu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nvvyfzmm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wcbyzjon.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2pdzuxwcg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jobjlrkk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xqjvzlgl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hybcffhw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dajedxnv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ilqhdaxr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hhlidnlw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dbtccwew.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nunpnnbl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sanujurc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zfbhskxd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvzjeyo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gvtlmotg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zbfgqjwj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dazzxmhn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2efxsrhmp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nkovpzsi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rlhnamsp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2oysovtcf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnklnsfj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wsldxtip.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rahpisjs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2syfswqvj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lobgvzdt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vlrnjrlu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2hccrkjpa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nvgpyiem.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qdtbazcx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vduffrlr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tamntiiv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tyjflcwk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tjepjrnr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ozskroks.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2lokdouvf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wytlukrv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2edzgnvyp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wflvycpu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mlenbben.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wlmuogob.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2azwonxkm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uebhafub.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2szhinhrr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pbzibmuw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bxqqotac.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2eqgxttjb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxltvo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2oujeqmto.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ybpnuzri.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ssqfcmuf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2robzkbcj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gcpxjwjp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2olosyprw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2leihftlf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sspwmvwi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xfslhddu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ivrxsjtd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2heutreoh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vtjihtiw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2trpgrumq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qedlwquk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cqezxdij.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pxwxkzgu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2etrtartc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qkdivtvn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dmgwflgl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnxyvym.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gaxjccxn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2avuwyhnz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sfjwigzb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2melbybfp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2roemnsze.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zgulvpst.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tkwqvjnp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yodxxiki.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2spmniyqw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ogyihpfl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjyznpgy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dkaijbjt.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2umsczbjk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xgcskxwl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2njgklwld.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oymbelas.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kweqmdje.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pfvaisrz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tkyypfrc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pqvfrqri.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wxyrdswg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2oirrftvy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2cdhztgyt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jivxmavt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2iyvopten.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxinzsj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wvpwuzem.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nmrhlgeq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gwwzsjri.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2snqkwxke.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wokqickb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ciwdtxjl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2drrnwavd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2kyygamwl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2apvdtmji.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ofxyonxr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rkornele.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdousoq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ygffwcgx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rlldvlyh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2clarbegc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ohvrqkam.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zrngrbab.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2pcxsvnzx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2muiaxjha.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tsvkqqaf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2plfmkdze.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aectpszz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hajrcpxt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uiacpjoo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pqolsxeu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqxgwtb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2omvhwdrx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2onckcgtg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kzciqplk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sjajlkya.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2fthvcbbb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ydnrcjoi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2bpxqvrdd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2swoshzjg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nmfdzytb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ohkkmpoy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zrrqcelq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mvhdbhja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drdgcqen.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cluiqaex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsdmxtnh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2oehswxul.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2enlnpfrb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pivjjsxj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2szxehsyd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nfrxqqqf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qwflfxtp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mcbamllq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ncjcxdcv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ighhyzji.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2urxrvxjl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2whuotdks.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2cvjfxzil.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bpnfrrau.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pzbfpjhx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ckrpmadh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ipgstykb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vewsthnr.html


<!-- 参考信息 -->