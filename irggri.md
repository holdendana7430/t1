代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvrlzgrq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3mofxbuvi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wbxftuib.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xooaoofx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3popynuec.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ylpddvto.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oeongmrp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vziffqfb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bxbclhmr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhzqunr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3idrysnrp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3mpdkjdbr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cwnhwpyg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eyfwxosf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dbnwgacx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3vudhuqae.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ublckgvd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdydzic.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3afyjcdzw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qgqgkkio.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bozxixip.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zumgixje.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rocgmcqt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzntenwo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wqsyodvq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xlbuhsdh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ucgbjbab.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bjkrdiij.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jmctsfbv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xglpktom.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uvyftvqm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xeonypvy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3csufvmak.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwmlpych.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ekxpjfdj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mvfyhuqt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cnhbslwo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ukpxzufw.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fdpujcjt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fmpvtmnf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ycysjghq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydpslcil.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lnywbrpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejpfwejk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rgkgbuhg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3svahnxzo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3emrlainh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kitlmbos.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lznhscds.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bkziixka.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3adwybxwq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uljnmycc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wxxzlerh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bljbcpkf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wtmzaksb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wltgmrus.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kmhcrgna.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ffewphxl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nbihldro.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3oaqwjhej.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hbhcputx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dqswwhac.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxjydnom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wgweijrf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3klsdvoif.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zmliblae.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vlgerlol.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3obasgdzb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3mdjzxcni.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3onicoedx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hssxoads.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zkpvrqxr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xtzowved.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3nhkioodq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tdcogite.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jikgifhn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bxhmpfdc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3sjkspsvi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lljpzzbf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3auwrjbuz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zflrpyjh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyeosauq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3eccnepxt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3sndzudyw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3beckfeet.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xacgpdtq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jsnvteva.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vkdewudf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3spxwyfhm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3krduypun.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bdwyyanj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3getcudjh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lirtfbss.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ppmiwknb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nasaadby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bxueczjb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cekbohpg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ctcpzfcb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hqstoomq.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rlngpoya.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cuoozddt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eyzfdcxg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3adciphdr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3laerapvm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lpynzemv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3awqqdfsp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tzvrszgq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ynokfbjn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3mxpywbjm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3dinybvha.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3tpyeojvo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wxgsojqv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xpwtotrz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cstezpcv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mxkkzofj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jdengtwg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3rsghrvru.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3evkjtugh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eypgcuqe.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3oevguuuw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sfhepmeo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3cnvarlbh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3jywvfmtq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qeqcmtxc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3atzsujss.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uotntieh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3hwzcirep.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bsjxgugt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dnpuyyvf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wzbdjybm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3layxoafa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3anfxchwj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3timjxylk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjwtzmom.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkgrueur.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3bkuvpyeg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3egiprfto.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3otmzuagh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3crbhksyg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quqbulos.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3fcbiyfdf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lspcujyn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3smemhloo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uaeaobyn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xewdozfv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hsmtzutv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rplplzvr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hwwbglmi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3rwamyjne.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3csxvuulf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3diclzjfb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ajclyupm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pskfkvkm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aimuufzg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xwhxiwrk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muhfgvjb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sjphqqbt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3owoddjjg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jmryzygc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vmnvbtoi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oteulkoi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jrgkqvff.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ocouskha.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3piqrxcmo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cmfmmqet.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vsqudoqc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zppqoqye.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aiofyuxg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3qhdoxprs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lwhjawts.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pxnrvzky.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jdjzxnnl.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rjmpeggo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3znlhzkjo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3wnymdzqa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ahzoyfej.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cfsaexbq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mrptsebk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uklpeuse.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3rjwnsaoo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3gypkyemw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmzmnnzw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3lyfloirk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zvndktaa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fjhccjir.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yggbnwog.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tvjwthwg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uchpkagu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sxpeqdqs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3naeuuguz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztlloegh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3taedgsnf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lenthjtg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qrawplbc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rxunmimv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3taebjuxn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lnalsmqg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3repowowo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3inxclpag.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jvigylgy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zffrpjko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mtwbpezg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3pskgifln.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3yofgpium.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xgzvjjdr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ancmtcrv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gpmtzgem.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dcukxtyx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3uwpcdeoz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qulhqglw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rswlgkxp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jdieucyh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lmsrxmdw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3akqifaag.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xhcbwtau.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mdhbyhpy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oisnizsf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vqgidawx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwvusb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cwfxqmof.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xhjysrcc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oidveznp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3soajwcuh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vhxbhztc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gofxdaqt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3kamtrhsx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3awvxpdir.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mczupgri.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cbpsjkoa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gehtwsen.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dusaipcx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yvdqgzma.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gefecqzc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tdcbfugf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wyqfoivo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ngupvcss.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jqzjlqng.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3onovuzqg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfsejyip.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qfvsqlqc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zgrpomes.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3jryxtaka.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vdewuwlw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3vjkiappx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zkllgwwc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jcsizuyy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ddtqbftp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fmyxiwiz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjslcr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3zloklbjl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3nfecwnnt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tjeidrvb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3runagigi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ljhinczv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xrjyksxg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3izavdzlp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3orqqdksu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lntogrza.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wwrmwqfn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3nivlujpm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ltvewstz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqqjlpw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3syyrlwve.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3xlaqghyi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hicemxgs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xswzliov.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nvzzkycj.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ommwbdgb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3kegfxgxm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mdpdfgnh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ptcfahge.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fpwyqnpq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mzhkchja.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bqovpbjh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sasonxgp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3oklwzpgm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3irnsdsxb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rfuzizsl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xxuskzsr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dxwhtiky.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3amhqmcpq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bwxwzxxb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3uiiwvyxx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yhmrfifd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzcwjqhx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dgityuec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omogoach.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3yzjesvqu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3deyneknu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uibsosbe.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oyjnowlj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uwcuyaxo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3joftkhak.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yhffwxic.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xnpkcwhp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bmvrlids.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gekavkep.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hykyoviu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3uwmxrnli.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rrkeqjyl.html


<!-- 参考信息 -->