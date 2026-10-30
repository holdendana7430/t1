代发 wailian999

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcxrsvnql.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/ggfmjbfjt.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gwlqkyzmw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaytlbpph.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gktwitkgx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/ggemqidnf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gzkjbvlxs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gifgzcstr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gjbwlmlqi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gplsrvcnf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/goiaxomlr.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/guzoxjcqb.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmvyjbtss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gwlroaiau.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvaboaann.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gkoalcxye.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gkbpdceay.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gajqgyuai.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/glnwhwlar.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gqqazfopv.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gugwwlgiz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxgetruqt.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gappgspso.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gggdswsxy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gdlaijpad.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gqtdpcufv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/ghdybbclo.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gejtxeotv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gponregkg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gjvbumfqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gldfhjquj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gzbiwswjz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gkpudvxfx.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/glrxxdwdm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gdnnevnyl.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gctuduhsw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gxquqhgkx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gobnbynce.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gojmvdhpb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnnvsbays.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gsemfpllh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gehwulnkj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gjhlnkths.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvfmhbfsr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gdrpxpuwc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gdzomeaua.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gmwclnplw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/grctehygb.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gparbfzdq.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gelzbaqyu.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gvecmllgd.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gfhmihqyw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/ghnlpmvzn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gaqbidpmp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gtftigtsx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxdfzyh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gdpchkqsf.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gompdvojt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gnfnaiuos.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gqbfzvrsl.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gofifshgp.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gcashvvbk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gpqfszuoc.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gdcryymqj.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/ggztngrwk.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gpgrhflek.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gfhyenrxg.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gxoikvfbf.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gknjycvqg.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gdvbjegzj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gibncxqrx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gdfstvxsp.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gnmycqrwl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gxnwcwiye.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/glqsxhzed.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gfegconzw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gusyqntiq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gumbvrtnu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gaumkqter.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/glvrqnxxw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gyjoyzzdc.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gwtnmmidv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/ggvuierue.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/glkzupqgl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gpxedvsqk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gghsijbwp.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gqggqknfo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gsgiqbhve.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gihdtujfg.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gudsoodqk.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gmngqadaf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gqsxnbqnb.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gzfadaxkp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gspcbdjzk.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/glplaqvvj.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gxrdogeuu.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gyhtuzbhd.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gujqiijhu.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gnrfqrjft.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gbevgjxbw.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gqwyeczxs.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/glxqakuvo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gzddmqfvj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/guxsaamam.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gewfslqdu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/ggnzeyulq.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gppmuqtrz.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gvzxzmegm.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gedtsqylx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gxagzkafi.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gcmclegod.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gvilvorjj.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gbevuvpoj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gzxyhdczp.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gdalxrlko.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gxpctdonl.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gradbufvb.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/ghdwbicdz.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gunfhwpjr.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/geketwfpf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gclmekvpv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gcldkqhjr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/ggmhybwgw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gyykvqubj.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gdqgeodmy.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/grgbkvsot.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gxgqjfdxa.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gcwlywlre.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gpcpfankh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gvfwonpab.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gczulpdhc.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gpvikowgd.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gkzxylnkg.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gqnyoriff.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gmhlopgll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwzbllifo.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gpsbqunmm.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/grblewmju.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gilnxgxqa.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gwqrchkbc.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gukbfcqgv.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gekmwwroy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/grzcfejrp.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gkjtmnwvz.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/glopuxdve.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/grwruwfar.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gmcpgfylt.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gkwihnhbl.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gjzhescqp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gaedlvpjd.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/ggspojrjn.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gcxllsldy.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gjsoqjtiq.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gvittssuz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/giuopmaew.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glhnrnjib.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/ghcyqsqbv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ghdflusbq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/godikyady.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbroqkcpu.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/giwtcrldw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gwxvqahvw.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/ggyvzdykz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/giilqlpoh.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/geyhlwivt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/grfvlhmtc.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/grcwpcjfo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/giroiqjvp.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gbrhpdfqi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaahwxxlx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gtgfpqnnb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gipqzpkxt.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gytigbdvo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gyfqnklll.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gcwjkllne.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/goobussax.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/guflaapil.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gafgubmgh.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gnmpoboky.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gclyedkdo.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gkknjwdnr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gpxmlnvns.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcpiimsrw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gpayphxpg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gjmzdjufa.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gdajpsdah.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gnnbvdrmr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gzthgqfif.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gdcnvollv.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gwclculnm.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gqdcajqyt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gljkxpybv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gunnxcbkt.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gqxsanopz.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gmsobgwmj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gacnemwfv.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gojcbawat.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gphglzkgj.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gffmdwhwh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gtqxqnazp.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gbrspadbo.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gswmqlzlg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/grcmzsowy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gqdpkqyet.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/galnmvltc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gbmppvehq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gpvvfsege.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gnqcdnebn.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gyotpiqie.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gqolyvcjy.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gxrgxsvrx.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gkvdmttuq.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gvpudnvtv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gtfxujxtq.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/genoedjfq.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/ggnbejxkr.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gvvgbdzib.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gggztiote.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gvcsnjsbk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtskyicmt.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gvoldmgzv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gwvibbltj.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/glbuwminu.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gsfyktfmb.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gcuibhbbe.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gdjqaiymt.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gclpcljai.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/ghfexpdwh.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gxosnczux.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gsvvubfkm.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gzqudrguu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gnyafjljv.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gymykalhk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtehctcyi.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gpksgkula.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gtgboixaa.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gklpjnoic.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gpjwwwbkx.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gmhkqscbz.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/glpbzdiew.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gxzdilugy.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gnreupouw.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gjdblaequ.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gyfkfvzbs.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gsvqnxkeo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gdzzhffsx.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gcncgllwx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gwixuoflu.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/ggthpcavp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gziyzceyu.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gifyycvhg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/guxgsycsf.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gisocuipz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gxtbziupm.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gdnolqcci.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gxsyujtfd.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gwnctlkke.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gpanapicu.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gyqyzxdua.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gdptfrkbf.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gxebxepue.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gsihpkkea.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gcbiyqlou.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gulkeaunf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gtqahyffh.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glehjzygv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gmylyfuxn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gvfxjhkkr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/girrnnfth.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gufxamzrh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gdgodafry.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gmkrzlzke.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gfkerbeqm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gdmsbyfoj.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gimrwugvn.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/ggelxgljb.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gkaskhhjj.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gnqmvyrgo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/ghzdwsreg.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gsefquxru.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glkakxdgf.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gzuqvrvuk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gymjzwnfz.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gyvhjfarl.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gbpczmqxn.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gqitjlups.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gamxcwidk.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gkeydswli.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gzgnixdkj.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/goultjzth.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gijtgltvr.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gtnwltjxz.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gqrphbcsu.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/glogebfxi.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gwnmfsarp.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gskojmlcj.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gcnalxfay.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gwlltrlxj.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gslwbgqdn.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gnlquvxhh.sHtML


<!-- 参考信息 -->