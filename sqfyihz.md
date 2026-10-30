代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdazafrlq.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfwuoncn.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtrxlgdbo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiceezqy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkjpncza.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gatjhazbm.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwitwwdap.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gqtgmknci.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giroynohp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbdjkpmc.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiarlogz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjgtvytc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gujfibljv.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtliobvuj.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gbrbpidoy.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghcgbzshu.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnjrntdl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhzbwtrr.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ghidovkfn.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvwsipww.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gumtejhvs.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjuubva.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwcoqqr.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gdqaexxkt.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/giklxlhmr.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grxgcgqdb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfvuwuf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemltdneo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/goapgwsjp.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyliuswa.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gahqxygcs.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gucerzhku.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoxrcxgh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpawtbnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqwmidkgd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glkceturf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gnoluyavu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkdbgcoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/griagiwnt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvqrdaar.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpakjyzen.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmoukxn.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzybeidy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gipximjyn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfqwlnuq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzhaqlu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfevunol.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqybhrqir.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/ghzawzset.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/glztkphtl.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gxbfuentj.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvuckfsz.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/glrnickne.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gimwmoduf.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/glklfzuji.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gbvndnrae.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzttqkv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvbrtwqy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdqhusceo.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyflncvc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdwqhjiu.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghktzrthh.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaawlepv.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioozxgrk.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gqilbbuij.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjvojvd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gcstppdim.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gsxeawcos.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/ggfdsphyf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztjfsfcn.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gyifggxew.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtlnzsza.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/giisdeqjn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gussetsbj.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gfriojusy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gghcyinjb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbbyldbj.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gozdjbjzm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqotxtgr.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmnvelm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkarcfrxi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrnnwmja.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gsvmedjon.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gahcuvmfx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gquqbbyne.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftojwfsb.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsvtevka.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gibgbojad.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gfcogplhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gfknrwmkl.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfcjuvgo.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gfrybfeyd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbwuxuld.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/grwtgxzro.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdcjjivo.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdteyvm.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/grayrkbqy.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gndjhysdy.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcfgdfqix.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gheqmfyof.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzjoylss.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gksnvixyo.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnpgqwqe.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gshuhjvqa.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/geeekzxxe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqfgtijz.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtsidito.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guenvdqco.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/ghuebpllb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gtihoxqxa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryzwhzah.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlszihuf.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gzlbdsbyy.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoawpzil.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gnnpxfeeu.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggupfchop.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gockcldsx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gwujeselb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoatnrqo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkjxsdvh.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ggmxekgsl.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ghvmvrmfr.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxdyadq.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzegqhiv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvlbkfez.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwvpvdbue.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfyrxsfnv.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwjyite.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggautxipr.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfffxopxy.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonyiednx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkallzlxg.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahflgybp.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlyejbxy.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gahoeyblw.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjtmcozv.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxzcfckn.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbmdzjuk.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnnmbgpjc.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gspznghux.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gznzfsmnp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhakwztp.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdhybmfp.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gixmuwfxl.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gehhtjgpx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwwxvjd.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwycavbg.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/guevksnyr.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqfvqipsb.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfshwdmp.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjquojvuu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gohkyklsa.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkytxvskv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmptrrpu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjlrceeo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfkdwwyd.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwwghbux.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddnhuzvc.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/ghjymnxbh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazjjqja.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gjdydddpi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gdqnubgbh.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gabmbyjnq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvzioudo.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gghallarl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxferebel.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gqfqlugbs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnkfxdgl.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/glygbejsv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gqthqjbpt.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gavopfemo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gykuaveiq.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpppwrsdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gnsdlimtm.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gplmjaxrv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gpiuczqcr.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/guovyssxg.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gjnttwdno.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gafsvacyy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gcvuttlfu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqhppnld.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijmvyrpv.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlvslefv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbmmucpj.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gwadutuns.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiegcpvc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/goztvxwup.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/grouosabh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtvgstx.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhgpzfmk.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gytvekrnm.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gudbgvxtm.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdlyauph.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmlijsna.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gbavouzvi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxprhls.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gkfugosbm.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gokkobpll.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgcihwdu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjqnngfmd.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/glbexvkvq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gygjxqefd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmacpgmt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthfwvudt.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gigliylzs.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfodtgsb.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuahuutf.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnymrcdzy.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gxvyiipzn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbodpkqqo.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gtwhbbceg.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gctxllgea.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gvelpxlbc.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqjsoqxkp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/giiylcsam.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gdzsfrbax.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gektnlbmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpayneqtr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvwwmxob.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gphdqbeaj.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grbpdvkbt.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gthkifgzn.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbacagieq.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gdlazbljv.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gsebvwmug.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrivebbl.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxxogfx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/getfmtzsf.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyxdjwqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdxdfkfg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqrshze.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gwjwdoego.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/ggxnpcwij.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gmacsoofe.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkugbaw.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvopetbru.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/grupfivpq.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gusmhwzil.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/glktisccu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupmvsrr.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gefanaqrz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/golgtfuvs.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gvijkatjd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljqhvfkp.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/glkwycwis.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gqrqtrgwk.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqxrzrvd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gmxfefyfd.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdojvpax.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/garauwikl.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/goyujgjnh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeozlnpa.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmcwcqme.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkxgmceo.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gghbyxsmi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gaplsjdwe.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gscfggrjf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/glnhftbal.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gbgyswzwh.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohpuyxil.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxzvwqvl.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/glpgrptme.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghjfwtlud.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwulaiti.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqcqowhr.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/ghduvyqju.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlkvorjq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiezbmvm.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghniyvset.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxwuvfv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfvensj.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnfcirzd.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gkgztnehi.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gaaciohku.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gupzzousc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeuplgnk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxzirmcnb.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvnjcugn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdqbahzn.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gktohneli.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmmjoxh.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gibqztivi.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gpucimfee.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatscjrhi.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmdbldne.sHtML

Go ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnziykkae.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grixwfufr.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gewvkrjlf.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/grsefkpgu.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslubprq.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gvwajcksr.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgcsqmcl.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvkbwxnb.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gyglnjbgv.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/govmchqcz.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gvngzzwoq.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhqczieh.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gybiwlvcq.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjtlguom.sHtML

按章节统计：
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuntxsjk.sHtML


<!-- 参考信息 -->