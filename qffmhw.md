代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2epegppsg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2lauwlhxw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gfbgbnyy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxaicljl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2azxhxrfl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2likdrsdk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jschwwwt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzommwrj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2naatkreq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohphchr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjarocsa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbbfabh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxknbvwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqptbcgr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpcrxssu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ruhjksgy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhqtwfwd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqnybokw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pzagmneg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gopirfwj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ijtpjief.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2myvyxgtg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jvqsmdwf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2njmufcuo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mclzkike.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2caasbhro.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugbmjfst.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uegvehio.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ndimkxho.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zzfkrrvm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqqzcbd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qefnnqwd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gbdayipz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmeqgqdl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sdqgqjsj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2utxqoqtv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ilbwyird.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkcbnvjr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gcmtjxmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbhynbzg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ibwnhoen.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kebatwoa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2cpubtrej.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mtvhxujp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2knmqsaas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lmvbdblq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2iidaxaig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nkfsyolb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2dhcbxbtw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2asxqeemm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ktogtpbf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2enuiknvk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qabcolqj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2svsvtize.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qljyqmlb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zgtnyfoa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2tpcktsgk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cerwvmdl.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nfvaolfz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lgjibdvq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2orroebit.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ocpmqozj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2tdumfmjw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2igtdtyak.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gysfgixz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2oayecnea.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2emkerxuf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2otqiviuz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wefarwrz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nseowcfg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2opkbfgto.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ufadthch.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rlnnpvgn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmssqrj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ewexdkhs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lphdnrpg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bvajvafs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xajvwgae.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2epydjcyf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbpipre.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ubaumxet.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2pxsaqpdo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dpiqvqfm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2uptutgyj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fiolyxct.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2oifeazrv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zkoekbik.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nnzrvuas.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fzntkmch.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2prmblntt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pghizbaf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mqgzxpwc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zottkitr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xnhhktmv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ierxwqdz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2aqrjzbzd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2pzdabvxy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ndiqchcd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vitczkhi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ykdqzjpz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vdulkblk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2yggbkmvl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2taahgrvl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ougvurzj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kvhvskzs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2uginekep.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2teusxxuc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dkzelblb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pzigunmc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2vkappkgd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cqckwtmk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uquyxpfz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cuoyhpki.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dfikzkuk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tfacmvch.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qkxunqqj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mayxaasn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2umcqfgzh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2yevkkxby.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2trmtfrqj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lfvohkac.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zaiegeqq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hlcjrnec.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nnatshtj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjqova.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ppzieams.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2omzusopg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wxpnrtda.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2zqaxeysb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnaipgk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2aofpnatt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cpnigtby.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftpmfpuv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ckgzjquw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xltkeexz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdjxwlnh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wugfqxto.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eovdprxj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cmytrzhs.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vhgtkzob.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2qogpnhsz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2adnrpjpv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hfstazyv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2iyefvwrc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2qrvaxgfv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cchhbmuv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2libkshay.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cugrxjjn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jgkdhpca.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2gnniogqq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dkbnufti.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2grjeugnq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xntdgfoh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2txbvdnpq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2esntpixs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oshrtecm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2amycobur.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gmpylqzv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mzxamsdv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fasyqwuw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rxpivzcs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gpfgyqou.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tlcxkdof.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2etefbxwl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jdorebff.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cbvhgobr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2elzsjrdo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2todbesnd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2fjefmjbx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tatnpgct.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mvjcmaew.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2spkxbmsc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ohbuayqg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dwickpcv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yvtcrnng.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2atkurvji.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pvpegida.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2afsgrupu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2foaggaca.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2unijoscx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dqqfruuu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vecbhlqs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nczdoiza.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jamntbkp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ibotkjys.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yasyfjji.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yrdepgpt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2zoudpwco.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zvllrlhg.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nlfxidxm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ozffrirx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uccvfdai.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qyiyspjw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2vhemfnys.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ezhjuoit.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bidmqsdv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jdufmdiz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mrumppyb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pjtygznw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rguzvfax.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ebitjlqo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrfwdy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jtgvzpif.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qnumxhsy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2brnggyeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zmvnvycn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2mpdpzjkb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2osboxwtz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zssmpjtd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2mxgouagr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kxzvvgba.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tudknmhj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2atqfanfw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2aqoesqzt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2drhchsso.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hlbswwis.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hexgrbon.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tzmossmk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2phtrgvtf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2keexyxqm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2brsfzwsd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zowsamzx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2utilnaqx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mexkpxnz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2opollmom.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cviliape.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dxigzqkd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xavvcpnp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2azvqyijn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2grzsznns.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2iznurikn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wtrwxcas.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ardeklig.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lznlnhig.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hegriuew.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xvguwhbp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rsatfimv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hifaryhu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2egyzeour.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gfnyrjau.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lduambcc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tfscbkqr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2amvqcytp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vchaarpp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qufseqrn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lqoqoppc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2xeysfupl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zjfckfyd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jtuxpgjz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vocriblt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fwnnrpwq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2iooymlri.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lkjigpby.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hrkftevj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ayoeqryr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2uprusouo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ovxesmse.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uuwqpqoi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ifidyjoq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2eizjicqf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qvyeivrd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ukecwred.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2irvrsjcn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kovrgfti.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2pfwacawq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rcyidoil.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvrtnt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnidsrg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wptjhiwg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nkyyxzjp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pefpajnb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2jahfxpib.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iuedufvn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2slnpgfng.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xcglfuvp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jultabsf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2lnyncsji.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sksnqpya.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nwyvqzgf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nhgucsrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hadgmpkc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zwzayvfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neidnhji.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2apluiyzr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2icrxijqo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jyfyjorn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xzbkicra.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2yugfinmn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xfbzbahn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wtpukrfa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2swoxeagw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sfdsraov.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2yvfjvsrw.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2oclleijw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pipgtrtv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zqveriwu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2eaedcmwl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2boculckl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fwuyqyzl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2nterzmgo.html


<!-- 参考信息 -->