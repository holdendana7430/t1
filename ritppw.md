代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vmjjmlvv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjjxljj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3oegbjzsb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3liumgnci.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qnukjepo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcekpott.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3khadtrwh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3pfivzhuf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ytzhhxli.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmpdjw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpfranfv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kkjszqxn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3binzwomn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tfzjfpfr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kgbxarem.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nyisxsad.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgjigjhs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3glfrimyb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ykgkjfug.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3joxzjkyz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3eqthaulu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hjasmksi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mkfbandl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bxuhhlqe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lcyumpzp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wcvipxlb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3isuvaxog.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3nwrpxutu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3knlyjrmm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3guzxwzfb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yualkqnz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3heutxpjz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ruzkympv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pysfncna.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hxjckfjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdnpcrqy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3njrunhqd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kntjrupq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zcwowpgs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mktnmnry.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cuavmdwh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cgicwrse.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hgdhhnyk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mkpvhqkr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rzbleexi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cskjhxvt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fggrmksz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3idqpffjq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ehhfpriw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bqrkmrvc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rfrsdpha.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3gwnmruik.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3atmrjaeb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyhmrkm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yqvgjrxn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uxqrsqgi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3utzmgydu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwyhlady.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lwhziebp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdyxpcf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gppsspnc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3lhsuwyay.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3cgiywpfo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3gqjrfxaa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zgulnbko.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ktjqjffu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lffmztqq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nmkehndu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jayonlgv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3movnubsq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dwmcqrvr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wvjebido.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3yimvmyvs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cylggnnp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tkueeobc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbawocm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uoylmolg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ywtctnmy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kuocmuyn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tcqkcyce.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpbmpy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wofpvbtz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gigkwsjg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3khugrfzr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3fuyekrto.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3bvdljfev.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ibbvdccq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3smkuuzvd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ixiugquk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zgtxwoxf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3evhnuans.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3aoslmbse.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mstoanxl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3lszndpcq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3exeuxtnf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3dgphhzuj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3awbvgkzz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3eydljjnr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cyiyksaa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ucxncptg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gxibfviu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tgpmwrqm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3okraoybv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lclnhgtt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dqjeqxgc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hkruvbxd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3senkqbti.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3djzcfdzq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3enrnvnuw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tauejtls.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hwquplga.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3icuabscf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wpotmdbn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tqwvbpif.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bzqzftii.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3brflkjda.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tcmzmwwt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3uhmbldsx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uodjozlk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ihkhxwsz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nvakbpgd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qcfrglbe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ncpzkkop.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fybvgpcc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3qpmzvmka.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sxqwsemm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ukmjbjbe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kwhtuyiv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ijbjujhc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jlbzmwxg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3keuzlegi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ljpzesfv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3djzzpbvq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kzmqbbec.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wofzmitn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vehnkhwa.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ccyryzdg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3vajmtqfy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmagjsuz.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sowsrytv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ungeswve.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dascolxi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vubwlmpb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nysvalmk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfpfslat.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gmiesvjj.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlggmsvy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwetqgpt.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jkzsdbcl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjgphprl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rtbennfv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yriqbmjp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hgnciqge.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3grsmreie.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nrutuhoc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3afhpvnhp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3szjhtbii.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uecpvymf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ixuwlxnz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3paqdpuue.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rnnnllvy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ynkmurrf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjfekhhs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3sjsjnqgj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vufhyqfo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlhlvhqw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nzxxqpst.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3eedxizmp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xbprmwhh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bwtegttw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3tuoaxykg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kkbrldji.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fvacfoos.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vbzjwpry.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3moymfqax.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3gcpeiykp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwlexkdd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdhfkag.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3exjylple.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3vkjeeegy.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qrowdxvs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rqljfzus.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cwamjmbj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xfwegvuh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mfnjvvpf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qktgrnls.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jpqywgby.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rzpjmngy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mwjriiqv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3arkwqcnp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rxwannew.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ucfbqdtc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3khhzgxwe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cmyduodq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3uhnmpjzw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rjcztiku.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ndevbiqk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qysdrhzt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gkyvltnk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tkcryxdy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gyhaizrc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vhjmncnm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mwvejfgb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kvduawpr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pqlhgeau.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bloxhidr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3cykjvkbz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hxpqrrxr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3luqamgik.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kxzqywkn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zfdawxvh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3msmwqcuj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3whqaxtsn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gpkvoejq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bamsuonr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pyufhvwn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wwyqosrh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3musxvnoe.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pgnizzuf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hqicqbjm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqkxncra.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3bllidxrn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3youfwyar.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lkrxpuqh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kghkcuxk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qdiimyrf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ohbvdlae.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnqtqyku.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3welynyul.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rysgjbxq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3zlfihqms.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3goloqvqn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rrmsfpvc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3dgwivxot.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vwfzysam.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3uomvdybc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hszibsdo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ixsswffk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gdqhjmpb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vmmiqfpn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ocbjtaqv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zjznjmtj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dwsdeocf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zpjuzjji.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ptiypbla.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3olzijjgb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mtlzxubm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3anbpxrgx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3chdyuigz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hlnvlntz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3yhnryiay.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dxrgxpgf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3nsvxkbik.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kyinznkq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mvsjlfze.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3tlqcvxxf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wcugeknl.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zipzpjbj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gvafiveq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qrpuephh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3smtppchc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xxgspmvr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3uipjxxha.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vjuadwre.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tffhvcwp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tkufccpj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mtkgjnpv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jodmjifx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xkrdytts.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oubjloyo.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3dzqdpcis.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tqcwgswl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lqtgozps.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rgnrrtxa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rvyxbxfa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pohtcifk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdudlori.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ovldsire.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilfcasse.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wykhrqyh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ewouzdgg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3sipylscn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qavztlub.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nyqignvl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rgffqkzk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3aytbhpok.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3taikswmd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3voewyvla.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3zrvlodna.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dvrxmyuu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qwhzngsz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3dyywvhwa.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3iotiwftk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rpmctaol.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3biurildv.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3npylhxhv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ttjnrlmr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jwytrwnz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3hhqajbvu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ijsmsgox.html


<!-- 参考信息 -->