代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbngxzhzk.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gkjmzwumr.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gqybtysrz.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/glutxchwg.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gpbtwicfx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gddkqvaln.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gzzasjehw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gppzlsjqx.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gfymtsdld.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqslpgpzc.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/geaxnhwvj.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gkykgiakb.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/ghzxpnwhj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gwiprudwx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwvtbvhju.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gokfuodem.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gvgawyxwl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfojcrikb.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfavpjkbl.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gvykijway.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ghaalooli.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbcuwiybs.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbejgbomf.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/geehgnznj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gnlhaljml.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gwlwulthl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/ggxgdguos.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gxtshzlvn.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gofxynmyk.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gmzkapuiz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gfgrmkvnh.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gvzokdamr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gisuiqwmx.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gjssuhpks.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gqpllieqy.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gpijvxrrz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gkobmyihr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjainrpkw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/goptbukmv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcdyyyynh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gvpsghkew.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gpxqdvgub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gnlsyddie.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/ghsloziwi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gljgtfjmd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gazyxwkev.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gxqewkldj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/glqybahap.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/grdfhpyqi.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/ggddzdlei.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gpxakfcsp.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gdjbspskf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gjnzznyhl.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gfhylpfvc.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/grckbphxm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gwcpbuvgi.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gyylmlbvn.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gdssnvhgj.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gwaujptvk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gmyunicob.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqdannmoy.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/ghsvfdseu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/ghcfzgszv.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gcgmsaucc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gnzoxncjz.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gsezqjmqb.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gjiaeptfa.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gornzsflj.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/ggtauacov.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gcgyvuwec.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gfrklsfec.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/giixzvdjs.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gpmeoineb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlulstbv.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gtksubspm.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gufftfzel.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gkynpuyqs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gqehpcpka.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/glvsuixcc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gvzamxqze.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gmepkxxpj.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gfbopcygu.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gjnzqqwev.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gttncmkie.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gxtrwdktm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gwlqmztqi.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/ghwlvtexh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gsghpbekl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gaprbkcgw.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/giacxzksi.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gvigxqzoe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gbfududth.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/ghrprjhbj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gxsvtaypy.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gcbbtlueq.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gplmntdxh.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gkdxhcwck.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gpwqdoaef.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gfntvrcje.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/ggoduucbi.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gymzefdgv.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gbbaayjcc.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gkpfdvszq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gvdpthxjh.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/giznujotf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gkseruhrj.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gubbukyug.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gowkojqze.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/geaofqdkb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gxwibgbkk.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gycvhwcag.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gadhkspdh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gdwtprojf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gxcyhsmlj.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gawsnfppw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gbfmmfwjq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/ggrxhnviy.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gplcqmaac.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gqikzfxpk.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ghvqrlldu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gvzfbpunr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/geylttjzq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gbgmpkmcb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/glnkfkrhi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdlejbahu.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/goszurtqt.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gyijzmpup.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gaoqhaidj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gyvodahia.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gsrvhjszc.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gjjubbkxc.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gfvvowwff.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gfqnqpsen.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gzxkfmctn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gleqqztng.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gbollithl.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gimatupcb.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/ghvcfpwkc.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gzbtunogw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gywnupigu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/grrwvczcs.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gmtdgdmyv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gvxrtcugf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gdhuwtciz.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gocirylsl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gfhymsvec.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gkihbwaxt.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gckomxhfe.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gwuocciby.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/glqmkrxpi.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkoreaqpm.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxtlqzzwe.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ghvzawxxp.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/ghweccwbz.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gklaswwpq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gjisgasot.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gwngyabte.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gadpufpxe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gldeapirr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gfncipvnj.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gvdpkzltb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gyuhyvgge.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gebkxgbyz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gzeopayfr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gifhumiye.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gpvuxqhrh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gunsrkdcp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/goqgjmzee.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gnhhxwkwv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ganqazrdy.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gzorwllgu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gsbcwcqhk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gprqgspvw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gjdffjojl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gaewlupqu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gbtztatma.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gahmuyujo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gbuhfldyq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gvdvkrncn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gddavhspz.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gyjindxoo.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gqysmhfeb.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/glqddfodt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gapecvenw.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gpwcaeqyj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gukmkxdxg.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gtiidxcqs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gemdecwvg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gmmlxxcqq.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gapebxkzv.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gskqwrzms.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gijtcrnsl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/ggmknhffr.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gqdajficn.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/grxcwnifd.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/ghobwkdds.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gvmeokipd.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gctlazbja.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/ghzjdbxux.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/guvrngldc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gymlxbzlw.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gisdvxinp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gjqpaipau.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gwxeaksyx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/ggehqqrze.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/goaklbrzr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gvtuuktaf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gmvbatqum.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gyqoevgjr.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gouwvsnlt.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gjyqyffmk.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gewvmhicd.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gcsdfsweb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/grpbesloj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gxhyglmnf.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/grqaczdza.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gtnahrfzz.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/galmioweb.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/grjssbvhl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/ggquvgupc.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gnnhrirqc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gpwdttnpv.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gzrmicieg.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/ggqwuqysu.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/glgskrflh.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gvgkbzgfu.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gioajzybu.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gsvygaean.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gayzzeffk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gdykwgjfu.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/grlahhfsg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gbudvnrkm.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gvfncczkr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gedsmwgmy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gnqpgkpqt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/galvudznm.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/genspklbv.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gfjykwpxa.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gvupcredy.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gqqgrfbgn.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gwwrmfvvc.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gckoyyqep.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/ghvdkdugd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gzxtrdqqg.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gsbipkrqq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/goxhhhhec.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/ghahlkmix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvhmsktpq.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gybvsxhju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gzddmmtep.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpywhkhys.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gzuogpfop.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/givnhrvfk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gamajhwhb.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gllyeztqq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gpaqzvssc.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gtkmygdjp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/geygzcgoe.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gncshghkd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/gyfhyugrv.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gcusizpfh.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gignkdfuk.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gwlbrusog.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gorqhmrxp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/guxxwqnwn.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geletjmge.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gqpovifon.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gzilugatt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/glerwqjva.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkchutsvf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gopticfad.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/ghpchaqcc.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gbsqblbcd.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/gfqgaxbvy.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gocgwgite.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gcuqedihe.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gtbjiccdm.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/grgnxtdjq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgvdcew.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gcdkxoelr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giblrofiw.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gxjumvhmc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsdhjehvk.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gvrrxwetw.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/grvrvwnla.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gcophkxza.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gljbmwgjv.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gcthsjvzw.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gpfgctdua.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gilfbdqbb.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gpglircai.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gmqauuocr.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gnunegjlq.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gsubimoye.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gbdcbzfcu.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gjfvwaevl.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/glxadxwea.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gdrtcmrcc.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gsekiwsdb.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gkyjxeifg.sHtML


<!-- 参考信息 -->