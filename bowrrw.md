代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jwvgbaab.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jxfdwtak.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ojixqmrr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uikecfwj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fvuoguvs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gkhgabbj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nculcaje.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmezkfpl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qnymxwlf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sattqaws.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2njttarkq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kqnzdnyu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mslearlc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwvbjpcs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oedwdxym.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zenpktyc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jgzcdhny.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lnxqfdpm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wsyakllo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qyriyduv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rprsszyw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ziojxlbw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jotxafxr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2idobukvg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htpmetbm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xbekqtpc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xswvvwla.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yjqabssr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jhqzxyur.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rntaxqkl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xnixmioz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2crfhjidh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzrgnf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2piyqctoh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ivorhqxq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dxowrnnz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wxwfgrhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqprapbe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oqzndein.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eytcneff.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mmmtbpkv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ajkvnjje.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2miiawrob.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hnndlpgx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2noasdgid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oomcgndw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2malqwvij.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fpoondyn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2vnifhqme.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozgxviek.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hobmffpn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yjpoeggo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2gvdiljvg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wyvnpvrb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2plwrjpul.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2otrdsmfd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cggqdpmc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bdtlckvr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nxumcjdr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ayaxthzq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nmrypyey.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oycptbjh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2euemkcut.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2elxojomg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2dcieicwu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rlyrsgmi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2goieadsq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2zcqydppr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qlwkhkud.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bngpcqad.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bhcglhyf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wzwlrchk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2qzjsdcyd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wvopklgj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tyczlsmq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lcyujjvj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2paglbqke.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lctayopr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mdeulhkx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wwstapnn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nfemcwcs.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jsieujso.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zncfbiez.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nzkujxou.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ndrjpeyn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eytvjoqa.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wgmciivx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ckjwtzis.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2azflgifj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jcntzich.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lcbzhyps.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2yekqruju.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2scyrngpd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pekzmcdl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2yfzhzvly.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fyokpvnc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2eobhubba.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2conylqyc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gdstehjf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qkjafvwe.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ciejluxk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wcyhxfmn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rehlgpqe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2erkvpswf.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2stqbvezj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zgcjcjoe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lpxwpmuz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gfnczwee.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rpkwwxnv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2sdpmvyid.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2szxandtd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rukznmfr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xwmubtxp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gclpzgou.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2tmielwwg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ubnuaano.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zyratqzo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lwvwbvia.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2doxhfyjc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cqlrjctz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2brirrxqb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2xrhaiymp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jjxjedak.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uoayalmu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wwyhiyda.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2dojsrdlh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ofocygpb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dxmfcaaw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ucxmvdih.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wgostabu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2whizznwx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2teppujft.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lhzuendd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qdrdbqwo.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zatahsdl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpkejpr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ejodwywa.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gqdrynkt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xpoosmtj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qszezxxz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qesqcuau.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kqmkogwy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2icjbfiiy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pyptecas.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2icxszpdo.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cntaiwpf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zdxhrgzk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2oxxxblqg.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iactjdbl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yhowkqaw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pitcygnq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2szozpyka.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oobzhnab.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2hxtxqoik.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2mvporptk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sjtjyyqo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vglxwyio.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhxlvjih.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2jjxoyhqi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2syhrqkfb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qxbofdwy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nxeiinqz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2uhxksczu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2umkctwnu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2swpoeqtg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2lftxbfay.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vcnhbgeg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lzzrtbyt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kaqefhco.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2niblhkbs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mfwxdhjo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbwzerku.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2msddssio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rwnpliuc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dnjkeelc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jftypggc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2suknphgg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2uqgzbkgl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xlpezlhg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lnbschzq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2srrwzvto.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fwmicqpj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2aussrocf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2yizyhnqa.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zpifdmyu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uqygkukv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2talzhcsr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jbjtzfmj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2gczxgojc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ufuvjhpl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2dphishxn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gxccuyex.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nvinauue.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tknbeecw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yrssaqpv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2fnrdumol.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tzmgtmdp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mabgegpw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mqalmipf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2taufjnpb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jesrxsuh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2lqhxgrfa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2mqylpnwa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdgulw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qlgxxhwy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gqzyciww.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2urwhfykb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2llrtctyo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2megmloxz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2cokoxynz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gmkkokdy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fadtxnsa.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gslxtqgr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mzpnulib.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hlkibkpn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wjzlerbo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ehbrzedc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jpysxcdi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2devrldml.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vtkkxjpf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hxxfuuhz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ohyjmkha.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cqcmefyj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bahtsavw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zfrfgnwu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ailqywia.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lkxkwicn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2odbmqfhz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dnzyqzjx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ybnfrjhy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2zmywxpyz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mqczfdls.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2srfjdwft.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lcyelhjb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gxvbnbbr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dlcylqbq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2clvamtpv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ivxnfigr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2lsjniscp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2cerobyfq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2wiewkkis.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2odszehvv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kuzoppvm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zckwwzdr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2sxhknyfx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2shbghfwm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2umspjlzk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jjfqmjds.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rtjwqdhq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2llztomfs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xnpiqldx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rgyubuha.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2foioxoxy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2psvhsjva.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2soijsvwh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2xmwolijl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jvwknxfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nbeijros.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjpust.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tngqzrin.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xysnabqq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mipfrzrh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ugkdsjjb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lphzgrsi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2bimyouel.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pnfndfbd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ufpvauya.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ynelpzeq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jnmiutei.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yloxhoin.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qnzbugyx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sjdpivfs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rcdrnkcf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2knkzhuut.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jgzuntyq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2snebuwpo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2zotsecdo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qqwpwuat.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hbvbcrzl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2onvulaaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2madtitpu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tsndweoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqinkuku.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pomktaav.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mfgtqzbb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qcicracy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2plbahrho.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrqtgm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2acqtkapd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nrwgoemt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bjluaiey.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2injylyio.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pcvanusn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xalimjxt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2hdhaweyi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qixlacoy.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2eftrisrp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hcjuaynn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nwganupa.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wdtybvwu.html


<!-- 参考信息 -->