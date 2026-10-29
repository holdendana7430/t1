代发 wailian999

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcxeuvdil.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gqpwuwaon.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gjahwegbl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gvvknfamy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gwomxuwfx.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gbtivqnet.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gsjsjtgdx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/ghcymgfnk.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gayvimhkw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gvpuxlfse.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gmmnonext.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gzrarxnwg.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gbfdkthzd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gdnhckexv.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gbqkbqdhf.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/ggldgdedn.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gzjaedgbs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ggcxtbrxr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggsaslytw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gupqkokbf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdclrkoql.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glbgejzhu.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gunuhxpdc.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbfcfcywo.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/ggyqmzkup.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gicylvsvm.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/glmbisqum.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gzyjvdzlj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gcpvmljdq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gatbjcodt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gyptoldpo.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gsrmhkkax.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gzmapsffg.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlpsdxs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/giroyajtd.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gkanoyikq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gmeoehulh.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gptxktrbn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gbididnnk.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gtnxrncya.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gluwfmiip.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gobtonaay.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkdtudmma.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzvqcwqdt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gukpceuvb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gmbuzbatd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/ggdcrwwqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gyctnjyjn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gqasxrfzr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gtjlrpwwd.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gljyahjcv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/guwisvuzr.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gpciqyqhd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gbstohjji.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gupjrkkuo.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gbnjfntop.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gxfvzpags.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gedcskrip.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/ggnlwcvvx.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ghcajjxja.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gkisdakfg.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gqiicplmt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gyqgnrqtc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gumsremne.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gbwhauyuy.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gehwornak.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gnushdmev.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gbdyznhkz.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gsnxsbjex.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gdslolanr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gbjfodxyx.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gxuoquexz.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gmjtsrzdt.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gushujjfm.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/grjnmiycz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gomuobzsr.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gpqzcxtyo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gzyubcwwn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gtblewkct.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gtvcpzukx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/ggpexgecl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gddnrfqpv.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gtuaqydbl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gjjhvtele.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gaxgduecz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gyccxkuhh.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gyywojihl.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gkaggsruq.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/ggntogubs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/glufusniv.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gbobkjgdj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gfodfvqtc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gsxlcmwis.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gxgxaveiq.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gamwrmitu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gtbvmqomy.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gxiffmzya.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gvdzvjeob.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gzwgazuyr.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gemwosumz.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gzcnjcjwp.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gzgbxcbmm.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gbpmktguc.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gkjsqcbqi.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gvwdyzexj.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gddpohtfa.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gmrzbiwav.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gzmimphkr.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gbvapcbkk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/guumnxoch.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gkkkkhveb.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/grdmigswv.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gqfqkeuuf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/ggwaccwod.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gugrzjbci.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gvocwrizc.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/guvjjldxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gqsemgmce.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gcrlunwin.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gwvqifhmx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gsrmonyst.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gogtgxalu.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gqnsrfufd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gfcokxjwr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gakjcafmj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gupontnxm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gjgazmrke.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gsehjkmzy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtzjzndhw.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/goaetsfpo.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/grqidnolv.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gnsakqlxs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gjprkfcso.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzxhsoiwh.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gdtwvcckv.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gweslbehs.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/giurorjnz.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gglvawwpw.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gxdlrluqv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gbnyzpcvm.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gtdpddfzs.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gukyzgcjn.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gccicrunt.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gjozhiksl.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gcoemayfz.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gqjrmaoag.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gkwfvgwsv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/glqloevnt.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gmydrftix.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/ghvwzdhiu.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gpzvpylpt.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gfjbcdkfw.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gjcdexsgk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gypjtmxmy.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/grqtilsmy.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gygcamhtx.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqovzdfdy.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/glxbsbinj.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gsnjtjnor.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gzvroocde.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/glciaiijt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjrdwboiv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/guecdubxz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gfxivuzbu.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gfctqdspa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdsllkudd.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gdmjhrzfo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gpsoznzrh.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gtvrcrbgq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/ggsrleqwt.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gqkwksbvb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gvgmivugr.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/grerjhxod.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glantxuch.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gbsmlzjpp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqwmkbsfs.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gyvuvdgwk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gfkxbgjne.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gjuxnsmkv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/goepzvmkg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gsbqegnix.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gymnsmtja.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gdzavdwos.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gdyivqwvs.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gduqgmtwk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gndwirytg.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gcvzgidno.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gurnqvwkp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gekasbrnt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gqzorbfij.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gpttgeslc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/ghjacrhrz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gicpovqpd.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gqxdimvyh.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gqdplrtqn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/guhlanuoc.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gfnggniiu.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gnxdewrdt.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/ggixoqefj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gxqxpxnwq.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/glnudhiya.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gmkjmghko.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gjbejpvkf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gffjsiwem.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/ghnvdmkur.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gzdvfqima.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gpywyvbfm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gewuygxqh.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gmddmezza.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gqwgmdtrt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gxmvkrqqg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gkyspjcek.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gpdlrfxgx.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/ggczeatcp.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gnqsittgj.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gyarbwjoh.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gbjphjgtd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gyjqdlgie.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gcipaanmy.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gxdhsetyn.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gqdmbywqj.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/grejlpyel.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gvkkxnaax.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwtiiyltm.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gtobeofhc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gcucuwncy.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/ginrvzead.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqukbthho.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gigdfpjif.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gwokzkbip.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gpjaebngv.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gxwylshct.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gdpvbgjpm.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gixhqykbh.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gvceysize.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gughlafvc.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gfbxtcqdf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gwlamawcb.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gfuakqgod.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gadgrmwac.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gzzfxjqkh.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/goesucxqw.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gdlwtiant.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/ggxynhcom.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gdbjcheof.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gkqsernae.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gomhevokg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gzjenjube.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gkjwqqszm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gjqsqnkuf.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/guecadiwv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gmdaianpe.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gtmrultid.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjgfubw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gxdahsljq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gijmiovjg.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gtkvassww.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gdeqopfhu.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gcvhqzfeg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/grcbdhiml.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gtrkvqewy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gqbjursol.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gclntucgz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gbenukmtd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/geuotybpz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gdayqfgfv.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gfzfsfykx.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/glxqchxpn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gowqoeqqd.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwlfrxdqa.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gyefnnflu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfawlfpul.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gumfiinqf.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gljisvffa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gnxxjgkvz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gnkwdmzfw.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gbvrsqany.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gmhiyilxv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gixedcpqj.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gvbwivgal.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gqzmiciie.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gdhalvkkw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/ggefaomvf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gjtmaplzl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gizlbwolp.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gyafefafi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbrbenz.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdjaxmr.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gibjfanhs.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/grvjuoyhw.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gwedrkppu.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gbtoxyapt.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gvebthiza.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gslwrahcf.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gyszripik.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gbfoflauv.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/ghqioxadx.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/goupnzdpr.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gckymvhys.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gkpsbclfr.sHtML


<!-- 参考信息 -->