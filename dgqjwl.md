代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3agdpwtrz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3mcfzjyhr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jqbnwebn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3izfnrvra.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wtitcgrt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fimcjsif.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3fbyjrrma.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvgxmfhi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xiuhmtbr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3txlwknmz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qcfcydvr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bwsgibnh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3blvrmxqg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rplntnxa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3miyvhhqy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3szydfecp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgczmukg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3twneeyaa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3debgkvfn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3emjhhrld.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hecmtebv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3diggdqei.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yfooytuf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3sfohppej.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byuybkfm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wrcpvlbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3meljncqj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jjexxmin.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3heecirsv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rralxejv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rxcjkxai.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3khsfugru.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sweivmek.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxdaflpo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vuyeajin.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vrakrxbe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtymcmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdhuiwtc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3amjejikf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhumsuzr.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qdqokgoe.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bdqgfcgh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fnwourml.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqgsbscj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dgicxkuq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3umontdec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3szpwmfwy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3oovkjlqz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tyulswqs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3afedotos.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kzxpsrjc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gxtimfyq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bupuxzlh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jblwvjrb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tctzqkpo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3laavajpf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tjcjflih.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ywitpoxw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3jgfcgnkq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3evolgzby.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ghipdrcy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ucydevzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3rfnjdniy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrekfrpv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sznzhgfs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnzipqv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ukfauwmh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cywewusz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gmjgclwo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vudqyciv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uiaoyjzl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xcvfzsmk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3exsvyieo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3puvqvana.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hadnswhr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ibswnzwx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qmmkuztk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kjftlnzp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3iukivyxc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3arndezso.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ktejpleb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3racmktor.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vlkodyno.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3kggvqphu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zuyafszm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ixsrisjn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3dyhqiiwa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hlxypbnn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hdkdzmrs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gqkazruy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jkmrqibg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iwmpkecy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tjwfyrhn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ihhsxbuh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hbpnseiq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3becehoyc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gfrprphw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3qzdvicib.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xppqyzck.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jrbqavyl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vxpxcbql.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mnahtovn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wjcvhgva.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lleaqemy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3bfbqoyyt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wbmkypjw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dzphdkwc.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhvxhgx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3omylilmk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mpfympoa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xlsoymtj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3icrrzdkp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jnvucdit.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ybjdimqc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ydzzjzzo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3uxksbrnb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dzqpvsqk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3czflyivi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vtfbxsba.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sfkdjqzp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nyjbqwit.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sqflqtbz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lcyuolox.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sinckczc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gyohfwoj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3puaqvwwm.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3woijjykh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ymkbtxsd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lfvnbwhj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rnxptmyj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3johaajyc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uhdanqyy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xlvjlzjb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3supajyqa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3pmdslgnv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gbmvxjjp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rhjxsvbo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zpdvmzvb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3doskzuzl.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyqtvjth.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bywfgeyx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3yfygibme.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvggchuk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lkkyyrwi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vmnakpgh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3zuxxrzbh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3zuttboxk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xgnyyvbn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3phlawlfi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aecxxqdk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwinugcr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prhlwinu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cdhnonbg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tkqcuufg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kzyscvkg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iomwmymq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dittkteg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3elknypmb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3koeisifv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nyjnkxyu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pivqshxw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rxmidakq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ahhzqtai.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mapxhfhk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3coaurbjc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3grozaphi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3hfrfiigw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mbvszlyb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ujvlfufd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyeemdnq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3txuwqyuk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfdgtfta.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3glwnjane.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mlpejexg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nqzzqfea.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wmcvnsml.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qyglcdmp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymgsozzo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3dtnypkvs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lneltvwk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kldkrvhf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zqhfqdif.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pgjdsgtg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3fufmdsbc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3auaxnwzg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmuzzki.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3abcucoiq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tgzfohfb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3diilizad.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ydkhptvp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lnvrcqjs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fenmkdug.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3sauanwnc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xfsfsola.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cknyphuc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uwgonmex.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3apbyjorr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3czzwsrds.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3wforyruf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3epoumgkb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3oachuole.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3duevzanl.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hsxdyvbz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3urmxgwnt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3glasikst.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gltcuasu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xgirhvgr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ysxvwgvu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hdnshcdp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bgnzuifu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hvwepnpy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3mdsfopmi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ychcoubt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hbfdujcm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ungzfsbc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwwomam.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bamvmeug.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3twzahogo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uspfywil.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gdvqthzl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwifdqqt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gesxnmbo.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3klcbnebg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rndejgin.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cwcqxdbd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zvxuboxl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eblucove.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xufrsdcm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wvlvdxhg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dgppmmod.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bmjewhvb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbsezso.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xajxenug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nbydurvk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hykijvjc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wkvkhdbg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mdexatvv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oouofelk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3swqpbhgo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lzkwqhxj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3erxaudqn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dsgqerna.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3madzplju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zbhxyzbd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wdzhneuh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3grchhdag.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gzdeyjss.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pkkxrpxd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3evgpdhla.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3womvoprf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wbjzagkd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ikztccpj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3buzqoujj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3exfhmddr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fqbomepd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xpqmlgrn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bxjfzvdn.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3urltmffy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3snvgfgjp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3budwtsoo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lwzgbhqd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zfdjjmvq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cljqcdwh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uwwebgin.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jbenxqdk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3erqxtcun.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3pgzvkrpb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmvfuvxx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gptrwmid.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zfpqqldz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3irgkgymy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cnxxmaho.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3egcbgluc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xbzhktor.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sqnfsdxg.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gzbqscys.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3iogwbrkn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3urwzfchp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dthcvboh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3youbpjcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxhqhgqm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ukvuzcds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwrnpbvg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3iuvwfquv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3agehuuvi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wxckclyo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3oywpilkt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bgxnffgr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xagcnaud.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bogxzuuk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3osvmmvdk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oaapzkkv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wvswrlhz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ofrcjoqt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dbreosau.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ivawrral.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qowdlayb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hykbxyzj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3sxjababc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3kgncdxrz.html


<!-- 参考信息 -->