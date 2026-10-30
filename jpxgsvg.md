代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gzetijwpd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnvwxce.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcygplwk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfpbspyt.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giofjxblx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grhbqnpfu.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfihftpbn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganeubjgo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkvfkvyue.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaqhathj.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpptnun.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvqjxgemc.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwhlfhslv.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkjaywhue.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszzrbtmf.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwlincxrp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glfjdfvso.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grdmypvxj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grekeookb.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gftmihzrl.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfyqzdg.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsutveysa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyofbgkjs.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/glruefcpp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgtxfuzq.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfurccqt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gidgtcmii.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gsjraiuvu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gnluytdvj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcltduwhh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiheakcj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsayehkfo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gnckdswry.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpalukhag.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfovflr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxebjnxv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdozudmh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gqlptrhkx.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geljbknth.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhecaljd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcanlfxob.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gosediivf.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatzsdngj.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guospiwol.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgvzqtjb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlvgszoq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyipyiplx.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggauwutum.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqytlcxca.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhooskex.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gitxgjvbi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/giuqqgwwd.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gocidcyef.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejoxngfy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfwtfara.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbtebaf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gblkjcgmq.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnqcyfgw.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gqffuubvr.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoxdeeta.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghovdrmgp.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjrwszud.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurkazizd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/ghwkookxy.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkjygzli.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtdsmzpo.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gjzhyyepn.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/grcyhbzbh.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjbtvobi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/grzenknwd.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/ggczefxoz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhnuktvh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/ghyprzdnu.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/grpzerpmw.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gieivceow.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcijjmajv.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxndiqn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnluwspu.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gjswyepxk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/guvmkrzat.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giodgogrf.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gmeqesevh.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgkbckqv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusiwaggj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/glttxghff.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscjmywiw.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/ghdlluzee.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gudrkrsye.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/glefbumpp.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gsdpagiqv.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/geuckpjwv.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndppxozp.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrwvavr.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gtxbufcdw.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gobmmkyqh.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrynuoez.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/grfvnjlie.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxixeouq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzlxesfv.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gcinksgdo.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gvsofaxis.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gsccvdbcp.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gthkqasfg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxegudaqx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/graroepfu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gbwkhgfoz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gsoszqfxt.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gstzypdnt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsqngtma.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbgaqclz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gkoewrouh.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzhvywk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/glwcvdsca.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvszoysht.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcbyyvxn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/giqjtrzax.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyrvxfkq.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcenewouh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnhzfuoh.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkrzyaxbb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gezmnduoq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glanfjnar.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/ghjqspvou.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gvlvtovhy.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqahzqqnu.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyatwylbj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcoazihh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvpqktbpt.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gyvzatqal.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzdmkncc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gcewkybjn.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnsvqkbf.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gxafydvhh.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gnacqfybq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdbbpnci.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gizepvurw.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmwdrwko.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqszjwlph.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdwfgdfj.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/glxysgdfu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopzrrewa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrwmgphl.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gypimempv.sHtML

f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkegqyfi.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxwvbza.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsgasrvwc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/guojuvfvi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gutnqbtan.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/golvphpmd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcocnjwcg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmimjpqhe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzyetjqo.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwudyulu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlvtxomz.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfypyypw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geepfdvxm.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gzmdysqnt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfxivsoy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjylqwdt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gbbpwtxqn.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gmihmegkc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbkjutv.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdpxqjxz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjhcqnf.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/grciwtzem.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gdefnqadb.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxuxqyjh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmooitue.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqdodkh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gyibcenig.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsiwpbur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gihcjljaf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzgpifgv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gmucteqnr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiaujyyh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlmrqefd.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsgfqkwb.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/guvupeuhu.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkegsmxtg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxyfzls.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gydodxwwx.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gcdlnzmep.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gfxohcfxk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdgtvuau.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gyrkqxwvo.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/geuvxscfr.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/girpeqdyy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gyoxpcftl.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/grwlvgeur.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoeumumy.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/grslhaswe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdgkomgs.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gbdnqgemo.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gjqauqqzl.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gkeiwokrf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfcpstcx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gboamkboe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gjaysmzsd.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/ggvypunwa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejkacqtj.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/goxoklgla.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/giohleoch.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gvmbjjfrd.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/grbysksfo.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/glvgdijaf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiqfhcyc.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/glpdpcjjq.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gadqtlltu.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlneeoxx.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gonlyynom.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfnlwoxct.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gumrughhe.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfcanvqgx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gldsagzyh.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiwdizrc.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gpjpvpjhc.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkmnyuphr.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gslitrtbu.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gadnnbfcu.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdhanbnu.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/glmheqyce.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gsupdktmv.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gfihvkhal.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtopiykf.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrqergp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/grntdnnpl.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrmgeqw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqrxdbok.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/grgbquabr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gauuukxhw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocyftun.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuisejwu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjakwyei.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxrblyke.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gostimyqf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/ghxraorjs.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgjerftl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxnimzvx.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/glforpktg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmwpkchln.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxsrlkdo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkfqwew.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gervdnckl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghngfukfu.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grnivbegd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gxzeshdnm.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gidahsonm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytfmncy.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkylmzdwz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gabsquiog.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gpobykhww.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/grclvsqxu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwyaqhpi.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gytqmgoph.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gyoqdzjxf.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqcxsruk.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/ghmfsgcko.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/glxbrxjyz.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbootovn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdtpuece.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdpasone.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkldyqpef.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmuuwtdp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfambkukd.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnixdqqrr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/golazynks.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gylwqomwj.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/glflghidl.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvazreqw.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwflvtcm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhpjhlia.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcpwrkbd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guywesgpr.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiupqnmu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpfdgywm.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gxphvuyvf.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpyaesio.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/giztsycwh.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxjraeqg.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmsuhsei.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqvuopgle.sHtML

Go ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbmlidoye.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gaedecmtz.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gteblrdyn.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgwkhwlv.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwbisidg.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gahjpmcpa.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/giyjpmeip.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzhpoygi.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqmhgbi.sHtML

Lua ............ 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjcptrej.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gqmwsgppx.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giavajhfv.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhacedt.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqhjbemq.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gkrupmkkp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/grrxgvcnj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/guilakxme.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrsnlhc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcszckgs.sHtML


<!-- 参考信息 -->