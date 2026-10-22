代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iilgqgdr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ylhyfxwu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tbpjxtbb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rqfhongg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oiojthko.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxozlgz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wsaawgjc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gznhrxen.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjyzfrnw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lbbtytdp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pktquvfx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sskfwrog.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dmewwkqy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qfcydkpr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pkdktkuh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlsxzh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhgnvojk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wheomfjn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivjcevyb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dpflwqpf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2knjknakx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zswyaxsr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bgzogpff.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2bvjqzqfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2htradtcx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xyzikgtr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqtjpna.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pdipqhtu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lhcxxjbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgqhzehq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eakwafyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mepkuxjc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wzuyqjbp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ehgedzcx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xriushyq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pbaqpygd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2liwkolql.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2iewllvth.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ybbdviia.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bfbsbzmy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ptgzbrhe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2apdlghdb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ehemvabz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zgiyqaeg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2guraccnr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mtdlxtni.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2idoadflt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ietueqti.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gfrpjeqc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xlriocwy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2scvitnzt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pyhwfdqe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fqmigpxs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnigero.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2suvrbhmw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2baawetxu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zzuwudtc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jdaliyct.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2kvsfbshz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2holsrdwx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wnecckvs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2knqpsmiw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2swokospp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bdnzfpji.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2scqwehmm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2whwokqkq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cvjmkyas.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gnwkrlop.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pctiktda.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2kxfxeayc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2kjgcxtio.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2tiycrtmq.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yvitxtgf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xztsfcsx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ojzewkzf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qpswxztj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hlnjftyt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2okvvcnmg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fqvegzpx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cgswzlmh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2dfehxlig.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ouexixdb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wtjvqcui.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2atmgjrjz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dxopanej.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hsviqsns.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2armrhcov.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yxdpebqb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2miklvxhj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zbydxaxr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ubydjqnz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2webaskep.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ahbkenwk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zhimkbpc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qlcjwrta.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ykiohmhb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jjyyozts.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2snfrrwxx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2jvpoblbx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ewfdykcm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hnzefwzx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ovzytlwf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zutjtyrr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hkowvmdz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vncowylm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2lrhiwptv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yrcojpkp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ndifkgdx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vfavemqx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2uigfsesj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2osxetirt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rvcticml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lgufaqus.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zpcpqwzh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2bkqiotdj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wyanabpw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jubrnutz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tiefbivj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pywnjnon.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2reexkqem.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2iypppuya.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tzjuoswh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2agebtkho.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lhlvnnsp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wpnldpnm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ysmxpjyz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fhcabxsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqzarnwp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vcvgpcsn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2zrwbjvaa.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vtqufniq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xymcbxju.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dsovgggk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ndzlgrpq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkalugeu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ojjxdbgj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2awhcygil.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qsdfhtts.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2whbvbxdr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ewsjmwmp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dwclqtdp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ryzzopki.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcnjrhco.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uwttvvko.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rmqlccbc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2agtwezua.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ztdyxoqu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2fbqlxqgn.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pedebgul.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nydbcfrg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gvwhnwnc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hknsueku.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2bgupzymy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nwckivtj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ewxqjtep.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bskaqzvy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2efhjfssm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgymdsm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2mbtdoklt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pdxsacay.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2uezpvbnb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xyoejyet.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2keclapfn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yxstmsvi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2uoffkfpc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zwrgwtxs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yuteplvl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pybdlecv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qaisjopb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2upnyuxoo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rqnckqpl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tbmxqvmk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mjidlpkk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jqtcvtdo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tmafnykq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yprgrmok.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ccthbpjs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vczhprem.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2spgikphd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mvdnxhbg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2snlrdwsa.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2svehdnoz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqkvst.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lvhfbylm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ktynglgm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ievhkrgo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nxwxjvis.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2crfgatsr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2dxtgnebs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ittqhqlw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2uhnidqdw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rrjpzfxh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2hloempcs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2thvwteft.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mdeuqsro.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2jpquvbks.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2oiocihhq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qejpoupp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2urtftgir.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cvkaeyra.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tlsntdvi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sxxlpahx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lgsetjug.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2egzehpds.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nyogxdjo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2orhdavhx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fenxfwox.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2cijhflfe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2mbbcjqul.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nzkeiprr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bqktjxey.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sbgzdsmz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xbhekkfy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2zsrrxtdh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cqhvkngb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbzicsjb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rftsqjxp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yepyysta.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxodjhrc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xdhgmefq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nxvsuquh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bzawgmsx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nddrwtkb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqrnwqtp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2itxcyqum.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ifvowdtk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tcnfwdzk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ngdteqqh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ldrkmayz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2drjkhrqn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gybxdpqe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2oyplewpj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2onlsnaai.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xzckjecv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ghitrrvd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2sxxsbgbs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2acvrsnkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uhhuemem.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rgegsivo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xxdjkoco.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rilfuttg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2khnepvvn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oapsexbs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2wzdusreq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zepyllge.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nlfujmcg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qedztelu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2xlpkticj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2oajvgaxs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fxonkoso.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2momxafct.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ocbkuvgl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wqrioxzt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jqltxlct.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ixwuzttp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ehtmpevp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wuuntrcp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2buwxpiwv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xxvhhhwq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2awphmnzj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ojmwimvr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hpabzvcw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iwvkqiom.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isddjqdg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrjltz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2lxyaubey.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kgnnpndx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2weyjjmgp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2reqcqcxo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fygyufkq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2cpucpowa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2cvyvzsqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jorkglxi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tnpyjhcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mchszqsx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qibnngbx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2exgrihhd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sjhggcob.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iabtodrc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tpvjukma.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mexokbhx.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lglwaout.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nibzrivu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ekqxvpcv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bkzglmig.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xazdsgxp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wswbadbo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vnvgqiqm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tixmvury.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hwqjcnda.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2waqgbukq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bylpaqat.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2smgjempg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oxmoucdx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wcpypqbu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zvakxwam.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2afbrxeva.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vteuqiyd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mrpohgll.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ijlztflm.html


<!-- 参考信息 -->