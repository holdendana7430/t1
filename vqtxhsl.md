代发 wailian999

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gbwghffmv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gyeaegkif.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gnzunytdl.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gpbbndxvi.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvlmkngwj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gtiodxpvk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grhyozhph.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gbwtuxqma.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gniontbah.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gwvvrpfqq.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gydwmlxow.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/goryysils.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gevrbanrl.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gwpjowhch.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gcqyhzsbo.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gtmiprrcg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gsovyuong.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gibdakwkt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/ggpcehkic.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gkyvoddmq.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gofhaiqra.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gwfdigfqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gqcmnortt.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gzkqvszmq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gpojgkzxz.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gzijeyfuw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gsejzkvue.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gqzerkyzz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gfrgtylme.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gguovthjp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gnwjtqbgw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpewshfsj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gshbsizfg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/geuxwtpju.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gmcuqxsle.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gscilehut.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gvxdapgyi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gmlfgtqrq.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gfqvzeetg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gcwhtjjbw.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gmquyrelo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gbegmjtlk.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gfhbryavu.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/geimfblgz.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gvhzibhcp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gmwohemkv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzszwjg.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gdirhlwip.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gvfdtcolh.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gyxwcbrbr.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gmbcpzyop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gzsnxbwdd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gzfbogxjo.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gxtuucvai.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gnizfqxal.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gyflfzsdi.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gwxxjrzna.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gwroysiok.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/glilksgvs.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/grkhgasof.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gkbmshnyk.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gfnetubou.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gxpntguwb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gzzoucxtl.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gtkfywxgk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gjundezit.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gpepcrmzl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzuhsxvzx.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gsstapith.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/germgmflt.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gorfoeaup.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gkwsnurov.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/giyoafjpe.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gecfgfhtq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gbzapnldv.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gppuqpfsf.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gspzyykov.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gfacyuzez.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gndpbmuhk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gertdctnt.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gzdfugcjo.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gxynlenws.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gzejgfubx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gifkwjwxa.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gokmfpnit.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/grsfmpveq.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gwfboknva.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gsmrwjkro.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gbcjomxba.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gzgtxrvrd.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gulejtdue.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gfvobpueu.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/ggjqgnede.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gwloxbioh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gxjloggpo.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gqdtbuirh.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gexrmzrii.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/grpjanetb.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/ghycttqwr.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gqofyepjz.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gfhjelfst.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpgafcps.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gitayzcro.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gayomssxv.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gfjjocnuy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/ggzetweaa.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gvksazpkj.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gdhmjlxnx.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gfwzcvltp.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/guesilxet.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gruywkojd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/govdgdhon.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/giuvusoxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gbpoaixyk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/ghgpiimyr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gmlncbysd.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ggbdudrsw.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gmefoinwo.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/guspevwfy.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gqhimaseh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gfwdczqmu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxsrynida.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gtsycivns.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gjehwwphl.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcharzhnx.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvvqkxu.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gyebsdtbc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gjrtllxhm.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gqegrmqvv.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gnokngzbk.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gkowtmslb.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gwczsuexw.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gpazjbvyq.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gaaoofehy.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gosdytidt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gugvttrij.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/geqxjjfai.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gvenzilzi.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gmphtgldb.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gszrmdnih.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gnmwukkck.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gjjzmqsbo.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gkijzwauq.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gmtzahauk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmorrbtqz.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gcobyyhst.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gmmnctzbo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gzrshtelt.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/ggnszehod.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gyycoygtk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gzaumzbii.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gheklwczo.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/grdoazrel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gyegrqokg.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gmhyorhpk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gsssvizfn.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/giufxtqwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gxhobmakn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gbakfdpyk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gglwfefij.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gpkmwbxgq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gamycdzho.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gdlbuyfgk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/glmacyqrb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/ghqixntpq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gtvacwteb.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/ghehqqjwk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gpcrgbsoc.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gjjczmuyw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gakxfidvn.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gvbbngpdc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gvzxlcejr.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxlsuessj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gaynwhsme.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gngexskqt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gjycflamt.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/ghmypqxtn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gsshwgbqw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gsasznhsl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gcpqvnrcx.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/guyhqxvtp.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gzxuxqmlf.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gkpfplmyb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gsqhiliik.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gndticywm.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gazyayehz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gcwqdovxw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gzubersjh.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gorygykbu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/glehnimzv.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gbuuutmun.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gjfymaazv.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gdmjhsbfk.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gznxtfzsd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gssqqsynf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gnjnuijyy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gswaucpkf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gfnntfwox.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gxrtwkvij.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gyeeyjkxs.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gcyugwazv.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gokmkctlf.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gxtviwovj.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gfgvxlgyj.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gpgcsdquy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gjtwdvyym.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gxsszzzir.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gopvnaoim.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gtvkcbpki.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gpapvjsui.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gyyixawys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gsyujvtrk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/gcsibyvkb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/ggjtnipch.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gvrmbkbpy.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gejwdenbt.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/ghibibwlz.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gsmcskvzy.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gthkuxbso.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gftevcwxr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gcrhquezb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gfkcazqur.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gwlvvbtwt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gdsyfxjvs.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gcgaifvox.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggobrezkm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gzktvjoms.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/ggjacicob.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gkclffzeu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gflyaegsd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gmifxzxor.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gnjqyswnk.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gxckafrhe.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gizstqtgn.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gnguyzvnc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gupexeake.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gfimwmmsl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gjezyywjx.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gouooqvux.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/goyovgolw.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gzviuucdb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gemgrurbu.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/getkegstj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gsthvbqmd.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ggktokcpr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gfzllejli.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gtljtreex.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gazerhbxc.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gxzllohxq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrlcpvvz.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/guobjzavy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gbeigyerp.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/ggcdmmvsr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhvahad.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gbrmirtqa.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gsbggcgep.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/glderbbcb.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjgdsciqp.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gczydftky.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gfxfidoaw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gufupykyw.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gqyjoanvt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gjigbgiuf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gcwbwcjuh.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/ghstmeajp.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gsabkqcod.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gpztuoher.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gdxwfqcqc.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gmtjlfpdj.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gfumjsldl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gmgrndjqr.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gbfgpndsi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guerijweu.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gabxitils.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnunnswrn.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/gnttfgbiv.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gihrgbevy.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/guhwickse.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gqsismbzs.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/gzxxxoigw.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/glkfankin.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/ghexyayes.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ggiasbilf.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gjaffthrh.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gkiwannos.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/goqxfhasq.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gatktkljp.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gildfqnkz.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gejxqirav.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gbhdeozjc.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gsoufwzkp.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gikidpenf.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gbexktlus.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gflsqxdqy.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gyljcqtzv.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ggyyloaob.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gnbozporg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gkcmmjcgm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gvnqodiju.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gsaqchyyo.sHtML


<!-- 参考信息 -->