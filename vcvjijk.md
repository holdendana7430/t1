代发 wailian999

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gavhcysez.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoclbguh.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gboonpstg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmnvzcyaf.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gbryfytkc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbswmkjb.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbsjurprc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjxrfpbd.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnkfmxpv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnskqpfdf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdqmelzgt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaxcrzyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvwvbjey.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklstkdeo.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoielwlt.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehzjcyhu.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxrdqrd.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqkjsnclm.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetrwbzh.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/glawnhbld.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevzcfpyw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmzpqbjj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqimdopj.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzheeahg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsnchxtz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwqzliqe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhnjrnmc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvguufvwe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjcadvtu.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gznqaukez.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/guxrafvja.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzqwmbtk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgaybund.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeztyapg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtbmmowjr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvwodrvk.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/geowwoumc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/grwoxrkyq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrchvaen.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giyyxxerc.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gznfhibdy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ggfbgkmja.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/guazgxseq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgvzxivu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gaiovrfak.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gacnmukwh.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/grxoytxkg.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzzxjbkj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleabeogl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbceyusbh.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gvndndxzs.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdnegqo.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gzhmhwesf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcktnetr.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmlsdgcn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gliwgttuj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmoqhlnt.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggnqsimnx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gygvftouk.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhiklfvi.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/grlntfosd.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoafesdt.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gocgtfcdc.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glomqtscy.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikuihimo.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvakjcvak.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gelvzmnkm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gozlzpyhc.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/grmxaobfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gedjjpvdy.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyyseszx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gatvjascf.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gpednadwa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffspkdpq.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggptkdunf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/guircxskj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gnctjjjpi.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmtjtzhy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoghzplr.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcxplwle.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxjjnpdqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gdndfwwnd.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpoyorm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjbjzvcj.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwsydavp.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrccioy.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuxnicwm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gimbrbzcn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gweudecgq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gvycphrqq.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gezcezzyf.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkixxwjo.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/goigefcdf.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbiwbqly.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gmidnesug.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczkpecwg.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjirdarn.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtiqiexp.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gxmvdaxwx.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gfzjnllnv.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqypvbh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gijraozil.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gwhyypicg.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/grxapbhio.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurcckkjl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/glmdhtqxt.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghozujmkd.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gbtpkbhxw.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyetaijce.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvudsyqwl.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/glmkzqjye.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpjjlhcm.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtzazkp.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwsasmun.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/geblgchjm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxtynodh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gmylmsaxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gsikawoij.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/glalsluzy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpawklrgj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngxutna.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gtriwocrt.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gsslqfooh.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/guorlpeme.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqmuaid.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grqomftos.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdnphfgs.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztocrqjv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcerdzltu.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gunrbxoff.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gzlimtbsc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gckddenof.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpdemuft.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gmexjqcdh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokaawypf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiourzyi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkhrdnoo.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwsoutyk.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gquukwpiz.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gugrqfwna.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gaourxkrr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjwmhbm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwoiuavq.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gpodruyfi.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdiqtiqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxctpcmnf.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzrhaqlb.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdfvihrud.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvuqkeuy.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqybiwrml.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gahlxaplh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcpqdqcv.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gelioxlhx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgfdjlpo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnqqgeis.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/givxtiwcg.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvuyjqyv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabzyurup.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxeatesy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/giskqzmjc.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxydrnoy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/goisaivof.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmrdlpql.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgbwyuxl.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gxwbvidcw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbrkwjpa.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gyylxscgj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhfllkkn.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gothnorui.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gourphrcu.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gszgfbloa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyochpbsr.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gibmhedzn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggipmfljk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjrblzdmr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gzmhqlhxy.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnwvqyqdr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcizzyfkh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbvqkqru.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/grhlqyhbv.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmbkfct.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnxyhml.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndkghrut.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gvauvsftc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdaqvpzy.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gwbyomwfd.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuvgmgqi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gddkowrca.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/glvrreqou.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldcwaqb.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gsyjqudok.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgrwkzpu.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgxyqzjy.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gyggaeukk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpkevjin.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gavadyqaa.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyyhpfcc.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gmbnmwqgt.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gniyfthed.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcjgrrxh.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gmrsmsdtk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gztbctiva.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzjmpnzn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgsgcyqa.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gnosmqwwz.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gjacbgevk.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gutuksvjm.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/ggldebrfm.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlwsbdw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gcavwapvh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappatmsu.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gekzrhqnz.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gzfxlravm.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyemqqopn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gomobylzl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrktxult.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzczfebmv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmfnhsqb.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ggivfnusi.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvoeftcfy.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gswgscbta.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhdmhsmr.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmncyppph.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqaiigqo.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gxxclmgpi.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwpordln.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gtdahrbxh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gpykydojb.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gdprvmjva.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gaxhaxdrb.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwjytidh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gmecqgtdd.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/grctuwqub.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gcerkycep.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxepxtvpm.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goumbrxiq.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/ggqpuwpll.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gisigrclm.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gevslopkn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxmrkbbc.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gbseqldph.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fanxiaobao.xyz/Article/details/gefpwnyar.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gthijxubg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gddwvkjgb.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/giuitxjqv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glldphrdg.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxdrzyae.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/glyyrrakm.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/grjjcmlel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbslbtyj.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gnoflchac.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmjppywm.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdnzadrc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxjzpcj.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gergeblgx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gzfbvjvkf.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gkzcqsvok.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/glysvywee.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdttlyc.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdktnyyjg.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gahredhju.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwnjddza.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guzegclyi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaexdqxg.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gflsgcgaq.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gaslpytum.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaflbounv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpxaraxff.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrqpvybq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvokgmgl.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorgqitmp.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftzzvuct.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gqowpnofb.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxeozhw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/grsselfht.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gotironio.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glqvpmqos.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gtbfmexhe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwxpvrnfe.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/ghviaryot.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gimzxmrxx.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gorzksmfo.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gifcuuabd.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxzuqcfa.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcuqecvh.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjgqnltr.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gtcmzdxjm.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gogmolvyx.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gchjglhak.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gtkqggyzb.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gzcomwfxw.sHtML

Bash ........... 80
来源：http://3g.fanxiaobao.xyz/Article/details/gxyuiccoj.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwttsyjm.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmutklxn.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzeddczah.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyapklzf.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvnufvntc.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzckfwzxs.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gqebyqhyb.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/grgglzqym.sHtML


<!-- 参考信息 -->