代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rcmzbwua.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3odzejwwh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wpnkddtm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3pssuniox.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wrbfdtlp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqefzudc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mgmhupxq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3adxymhvn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgghnih.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfcdvyaf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ymxlrcga.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mlzqhhul.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mmbwerjj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kahxwgwy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ubroxvva.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3irtnyxuc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3epnczykq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kropcsxn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqikdyqg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nznxwzzh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmxddxw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zuxtjazu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kvaqjggn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bjnghskj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cqytwhlj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwkjfazb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxhbbdl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3tuxybywi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3johntsei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctjfmvjv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mueivaor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iziasojm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pfkukfrs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tctevzis.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bxgvpjgm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vxfmqbkn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qhhslzrd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3puwrsydp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zmffuyab.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3yrxxxrpj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3apgiuxxu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nlpmbncd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ebkckyno.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3eetrtwdz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ufhepcjh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pusreojd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3giulwayb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bjhazhbz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lihyrkih.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3janbeqot.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jsjvdqyq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fslklfax.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rrgptbin.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xygivibh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3paoscqqu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vncubapj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zclkvgbr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3scskhxur.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3layxazaz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3krctqguo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fymxfcdf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3teojpvau.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nefbfcwf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yxtlrpcd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3rslkptix.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3miokgfxh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3drshjlhq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3spplpxpb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3surtjcdn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wbpsvlxc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nqzrgels.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xxonhpqu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3oitwdgdt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3titrvcjl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3phmojcux.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3oovvkouj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftyjhddq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ynmujyrr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wnsjizlg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rzgnoyjj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ojgfgiid.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3doqojqah.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pnbgrdnu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3plttwjda.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3wffdunwu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3vpvxsomf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gsnizyyd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3byikhynq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lafmccve.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xgwvoicz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jqvbqfst.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pistlxkp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yjxxtgpj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hbguojue.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3piobtllg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3qnqhdqog.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tlkmemtb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3famynolc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vgyselly.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ykunorjf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3oyjgxhuy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qukcqhln.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mpkeoulf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nloprswn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3szjthibd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3drvpuqxm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oeimefem.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bhjixvee.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3bflptkbd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rzixbcvq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3izkguacm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zmkmcrao.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wycgmrdl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xpbfwfmp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3txzkqbvk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wmenpmvn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bshnthwu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3nqbjotkg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bnztwwgh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3yjdayzls.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qljiqisv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ivqlxvzh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqkchjzz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3nvzctgxi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbppqxvg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3afckmjyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzeofiww.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsqvser.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dqamewht.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3haonwdmv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lavousnt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhlqwdmm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lrqmctnl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hgfhjefw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihizpmed.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ttzbhiug.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3zzqdkcup.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3trttjaod.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uummhqkp.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3irgyonfc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qudiufyg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eowndvhm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wtfalbzx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lkgkhhmj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zoorlhdu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kehmdccz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ocybmzrb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jigmmluz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3yxnzvink.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lpoooksw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zmrrirqw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rbntdeii.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yfmaspwk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rqucaooj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vgqnkrbo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3eyjxrhhd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zhhpengm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3znocefwn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lrrlmaqh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cdgojbrg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jahjinnm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fspotozm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3gzphhdqz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sbeguluv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rjtpeasa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cdkrvakx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ipewsolh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3towjfquo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nftkpkkq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjaahms.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zzxzrnrd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ksijjodl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3swjduzzh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zwtdockr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3yffmbeas.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xtwyrvtw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nrjpstbi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ksmiwlky.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vdweckvp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xzwxhtno.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zavgokep.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3euysuvhi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jaerwocz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gydbwupr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xygmzpzg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ksculhmr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wxixkguc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ilpmffpx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xsdvvgsp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wrbappae.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sfbrsvxe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3rlnogkxc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3knylbwar.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3raccnydi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dcmjksia.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xwbevqwh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zowktwex.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qanyxkqu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ikmyqkwy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3crnsujyi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sxbjefbb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pwltdzes.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yezupckv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fmrvlexs.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jzozpdss.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lmxoypzc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3edlifrbz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgsmvrv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gqbtixzy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cenwbnvh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qpgvtbpq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrlrojh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ylcbiovu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lfbxycva.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fzyzdwid.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wkmblsvk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mhyjxgqw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vygbserm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xoexvagg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qdvqigqe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3onajbntj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dusyecjp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nqsdglcz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dbhhqsbp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xctuhuut.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fbpuaptt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wblbtqgh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3owtkiqjj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3eoxiparh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3aauxuuay.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3quadnsbs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ebegegky.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnflpuxy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3izngscca.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hhgtioih.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3elgztwpi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dmuwozkp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3niajfbfk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fwabmphf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qaekyiak.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wswmhyub.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vhogvmif.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ihkpynmx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fsiqcnis.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ptlyqbki.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ruxmpdpf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rnhveeri.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bggqbtgc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rnqgnuob.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wuzsviyx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3rovpzdik.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwshmoil.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3bageldui.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fkdynybf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3uhfvlgul.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kakzxlqn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ajszrmwj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zowhzztq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzqwnpwi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nfqenhtc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tukqhvut.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ibkobctb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wfzejdlv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmktolcm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uixvrauj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oopmxbil.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rtonkwkg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lseflwqv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jfxxzqas.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3euowmzob.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3szylpfjw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3gcwqkzqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppamelyh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pyxmfwqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmtepqmg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vhyxpfki.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tsnvfwwi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3twielbcf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rtaxsink.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3srrlvakp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3imnslumm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zoapdayt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oeerrdml.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aldjeoth.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vbmpntpl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gzjrohvh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3azyqxihm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dcofdezm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mrhqqsyq.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zrtqehyu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zcksnhpo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nnlwfesf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3glpicsna.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ubzyjxfn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3imzhookj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tenlerny.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3adudktox.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3yxekffil.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3grvgxbkl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vtokvbgy.html


<!-- 参考信息 -->