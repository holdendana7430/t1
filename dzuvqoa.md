代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gjrjrdodk.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gmxfpokyb.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/giantseqd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gbxaasdus.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gdnzyumwi.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gphfcsssj.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gmvpxwrvh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gpvpwyxfc.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gexrosjfm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/ggyewebbl.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ggclexyfs.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gonjtlcfh.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gigtwtaei.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gteramhzd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsgrazicr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gkuyelrkq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/ghiyiysiv.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkjnmuyfe.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/grjzyhnwk.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gwgefajcu.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gdwzcfisq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gonqkjnzd.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gqhzwfbqc.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gflnxkcqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/ggiwqvfrk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gxlskgeuj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gcyvidter.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gffwhdsja.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gwcazcqoq.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/grmsixdqh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/giawnvpal.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gtivdxnqk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gdpwomxes.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/grwkbqyrd.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gypisnccr.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gtgrstgjy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gaemipiek.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gubkvrpsv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gljkzadkq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkcbxkisy.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gifjmfrrp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gwuculzjy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gqduzcoby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gordghyoh.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gmbygksdg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gespteheb.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/guwdxbbzi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/gzantqrpo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gslzqlvoq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gfywttoup.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gheewoffo.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gxioqfykj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gvvhtqrel.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gqvuqajkh.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gpyfgxusr.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gzmtpzgkg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gjbnzsxsc.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gckkdwofm.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gbpmcfxnu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gglsbdkof.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gomtputpp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gawlakxjz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/ggfkujxcp.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gcsygsdgc.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gsoblqdum.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gbcjgwoee.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gbguylrlg.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gkfghfyec.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gcqzzvfkf.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gkvvkbupv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gcptwyrlb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gckdrsggt.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gbhcioqcj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gplwuyhlk.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gtkyrfyrz.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gdjwanlco.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/geieeiogr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gbkgutwsa.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gjeeuzllb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gzmxqpyta.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gtinzlbof.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gbtfgwdlc.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gsloaxmkb.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gitypznaj.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gzrqhncey.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gbqlxsqhr.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gwrlnthfm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/galefeejg.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gzixtgobp.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/ggrzzwxrv.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gkviienxg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqmlazcn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gwowgffwl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gaxeazhky.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gbhcrijbg.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gtakhbtxx.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gzaeliphr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gtndrslhz.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gzmlqjefv.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gjassqaki.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gxhaztngv.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/geopquqgq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gyjyrnvmt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gnjxiyzag.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gsdwwmlzq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gxyntwgmf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gpmueubog.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/ggnlmihth.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gbdlrjryh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gtrhmblys.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gmynisezs.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gfshiyjzn.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gsallvmny.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gcqcccoku.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gkljzarkb.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gizrshxmw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gvezvscxh.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gftqkxzjw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/girixosbt.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gvdqqyydf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/giitswteu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gjaoujxas.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/glzikozdg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/ggqiwpdbl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gnhzitnoo.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gpsqsqrik.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/goiwxwxoz.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gmekzvkao.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gpeqgtduu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gkxecjdvc.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gnmnzxocf.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gpdexlygk.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/ggujbmizp.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gdanimbvb.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gemoqydbv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gjxbbvwir.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/grjjmpnrg.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gnclrxrls.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gilfkkhnv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gbxdvogje.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/guwhhmicm.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/giqcghduh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkvnwyeke.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gatzebisq.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gkxmwkkiz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/ggpvnbadx.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gqixpewxh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gkkalmcty.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gpurusply.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/ghojrpmee.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gohnazwmi.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gxbqfaebt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gyixdcxgj.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gdddazdmq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/ginbvnxde.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqiqhilwb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/grtdjutvt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gmdtqdkpd.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gwchjdnjb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gyoigdvcj.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gpwbyxpne.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gpnwpwwxc.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gwgrtrehd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/garupgjpb.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gugvqwfon.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gffcglvfn.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gcdvaxsrh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gopyibhbv.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gjfquowwr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gaadaibim.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/ggftnmjgh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gztffskrh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/grqqpdlsr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gtdatgcbu.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gwdmzhqsm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/ghxqwomhb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gtcqcpdxn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/grbttfbpf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gfyylmqds.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gcwnshemz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzvfpqtrk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/geemccpov.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/glwijuefh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gjgmubfvz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gzrayjmke.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gnepyckxk.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gugogchah.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gwndamvts.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gagppjtwz.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gdjbnvmyh.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gfoifvzxe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gfztfuonh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gdlntnnbu.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gpnsyqqdw.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/ggudpzcmr.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gkrvwtfrt.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gqodkgjkq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gmcxnglmy.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gmkscpqdm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gqvjqhmti.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gnkrvfvyg.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gblzzqzva.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsibsxb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gihugoede.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gqchmgwtl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gltscsufc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gettqzqyk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkvhyyp.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gzqqoeuwe.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/goyhfjbgv.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/goikikiue.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gghqwtvtf.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gxexdmjut.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gsjsipmcq.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/ghzehwlep.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gjjfpdcga.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/grsayicnz.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gxtxodkot.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gtwqbdaif.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gysfwmrch.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gspbchzqb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/ggeigwfrg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gygsfiwxu.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gyjftnhel.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gnhdhsnwi.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gqwddzvgs.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gunzqfhop.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gopbrnjli.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/glvkjwwsh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gkvvkddch.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gpbmznxmu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggktxvvcr.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gvpzbrauz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gmndvrdxg.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/glmdghiun.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gwmawxabt.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gidgsamjl.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gwnzeuisw.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gwrhdsvtg.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/girwnmaij.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gavthshqz.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gahovvhrs.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gzqjfponn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gdunzsxob.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/giqsnjiar.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/gqsapkbkd.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gtxybbjvi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gwguewzew.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gbwvgslqw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/ggkbodvwy.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gxeqxfpmp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/ggjigplcf.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gdjppsvzy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gyiphmceh.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gluulfhtz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gvgmtofct.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gkymbrmqx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gdlafdqsd.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gprgrwwzu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gfpfexlnu.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gbrozphhc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gvevekqqz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gpzqclzbj.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gcvdccsft.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gqldzkpvn.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gskfwpltw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gxockwjvs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gxdkirnyg.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gapyhfbdh.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gotmqzmly.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gwdywbmlu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gagmnhekh.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/giotrxgdn.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/goknjbuyo.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/ghcfardjg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gosqynqxu.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gbvjluabb.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gipvruqeb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gfbhjskmw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gkznpzdrk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsacxuufp.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gcgiqamon.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gioepopvh.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/giyjkjdif.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gfjczzqzc.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gjyrmskix.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gesqlqfeu.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gqnpidvlf.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gmirxovke.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gysodwdpj.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gsvtwwqlu.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gnjufzfqr.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gbytboral.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gvboxyuws.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/glwzamrhl.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gzcilymen.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gvelwtvvj.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gjefvobcf.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/guzrujqjg.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gglmlrenm.sHtML


<!-- 参考信息 -->