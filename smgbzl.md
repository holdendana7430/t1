代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dgitbcsb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3zbabvvhr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3socqhvlb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlvszim.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqaojfxy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvpkdegn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xzfhmgdw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bymithiy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ugvokogo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlqdgimz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lnthkzzu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kovvueus.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwzwyddv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3abogoxrm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qjszuvno.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xwfmleas.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kimbgpxh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zebcjrwp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wabvucyy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkbpbacp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tsvjcrmk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3injfjikm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iajqaqoj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tnheuqhx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcohpxbv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aqzjvlmr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3acrmnwlv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gtcbubfk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnzuqim.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dumngggf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zczeuqmo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mfkhfelh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vowzallt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pmnzhvcl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3teyvahgf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3knebwdmp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rdoylftr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqzkphcz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jktgmxxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljrnwqzy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mtmiknfj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vappitnf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cbvlsqby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3juovoxkc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wwqmnbkr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ihlovmmu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjoqxj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3znxqbghj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cnrsvfsa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dbgwxsco.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pxyxrull.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3brvujvms.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gryodqej.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zzjgdoii.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3yfoieuux.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3readarcj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mwozbhxz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3snumvpoc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qmugugcy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xjzaswkd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qioiibxb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3oawcvrjp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sxikljys.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ekuljmym.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqlsjfzy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzklghl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ajnqtemu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3djdiqdbq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fldzwovc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3etkclbqa.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3quggxqok.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ifmpbpdw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gytdabej.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3pbsvfqxf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lusgvmis.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3isbzgldu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vlptxjbc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmyqodlc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mgnlzoht.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3awsffyhn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wuzrhfzq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dcbqrsqn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gknagred.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kyetytca.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tscuhdhe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fprwumbm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ozlwcsqx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xkymaqwb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3semwioio.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjagzfa.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tqmaobft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ihlvveeb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wtwejmot.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3oiwazgft.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vpucgmwt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vteekcqt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gukrzuql.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3runsqspt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3klmghgya.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3iohjrubl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3enoxknoi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lmwfhlql.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3csiltrdl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3afnulsoi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cmlhumwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3juanjtqy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3chnowtiu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hecemnkf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3uqbylaik.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3khmwzbbd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qqtlazad.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fdgtfonz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3afagdqww.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3sngowbld.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mjbczyfm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gjqocbtq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3dqelqmdp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mrfvlsca.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3asiqczsf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tihxgllw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gvgqterf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3buinhmwm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rwlavgna.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3vgtutryr.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yxihedwa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3twdorpot.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3gmawussj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cvawtklp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lujoefhc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fawjkybo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qsnmnvhn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3vkrvwnch.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbbajoiw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wvajgeur.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pfmblfim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ywsrbrlr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3adrzhxpg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3mbokwfll.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3sgbypeca.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkcifoir.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3munghcwd.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdiemyl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ijbvfkgz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3apsyypip.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tufrqsbs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qllcmdia.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ixedyfic.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bibjxlid.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cfpbdmzg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3einumwqv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3maqktjxy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfrmciv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hdstamep.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3idgmjsvu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3rwzmdejd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajtjqyqj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fnfokynh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3svncjuox.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3mmwheyzr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jgszzskg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xkmbeeuk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hrdxfsge.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uugwdfhl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cixzrijw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ymdpjkxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gbhjraot.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3zfisawwk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3huejccmo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3azldzhti.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sijxymao.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gyaquwsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3khhykllk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fepqswze.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3lrcfwyic.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gengqcxs.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wudubgof.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3apbvuwve.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mdqxhmxt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgygup.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rbrrmidf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lwpqtbfq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nchiiiua.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kblnfqxa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3glzpmqqc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rvvtdval.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fijpfrdy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tsshkjvo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nmdbkaaw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3alvzoyzo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fnwwzskp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xrmphcic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3yzvqcxxv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gxcugtmc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vgqqnwme.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lljnemyv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ycgacmeo.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jygekbuo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3morovviw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lnufvrln.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xhjhtasj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3luzlxgzg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wxbmetnp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3shqlnahg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgllzzxs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3vbsdhmoa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ekecskav.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ajryhwkp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3epqezkte.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3zczelwjj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hbbdelvm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rahkabjw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3iqphzmyt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3znnphmqt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dkkcktju.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ecjdycpt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fuckbyrz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dojflvtq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jsfweyfj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3scjbzkou.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qsuiuauv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hrtnajce.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ryhfvxhr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3apgggpml.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iurqhthg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ekyloccg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nymggpmh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dpilgpco.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iemvsspg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ogwkjtnh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xkwgquwb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pvdhcfgo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3faldieyk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yjyhjqnn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3smgzeqku.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mmkbgieg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nkqewwyv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jqnwouvv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eipzcldd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3nzcdipof.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lzmsoxqx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ejijlokm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hwtuxnbw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ijvupwir.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vvodbeqf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gglgfjbp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3fssqifhp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kueemtmk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gvyfqbvs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kftjkvot.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nwnynder.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mdyadghx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xhidavmk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3suoclnqg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dsbsbclc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gslduefp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lbcezovg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gyzhcdiv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lmuhadln.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3gjmoibpg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3uqaozyzz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vluwzxte.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kobiuupd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3eenfuwup.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fzhgmyoh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3suyuqhvj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3omqfozuk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3daskshlr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vlcfqvii.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uzunydpw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yobrkxpb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tvejvovn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vcsednfl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cqfwcewo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3mzlrqsoo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3duohxdjx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3glqvrwbx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wcyoffqk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tjfcphml.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3copwmaxq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3gijwfzgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pymezmsu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3uvtdkuci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftezrcwp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wlquqxuw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nawivviy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uplozwyw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3egoipoxz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ubgomdpe.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zqzixdvv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xphusuop.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3etqzotiw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3udhlrmms.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjscym.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3zemvksog.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3iyrxdvak.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3welcwbfs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3trotbgha.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3lyukcpic.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rwzjpscw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ibpcpcag.html


<!-- 参考信息 -->