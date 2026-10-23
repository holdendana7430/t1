代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nvylhsfq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yjorwgwu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ecrxxpvd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3catjjovh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3bahlitay.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhacquvp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gyglkwda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vetlvvmp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gppqtncq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3atslvpfs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3sqkvveqo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3egfngsvk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3hpuqdnzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlelisf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjjmyxxy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3seshvjdy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3sosfkeoi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cmcbqbhm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3khfqlrka.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wtjrfigs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdqittnq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zcduugsg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3znqsuugf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ooemsyyx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyedbkho.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uivogmtu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wazhmxai.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iizoykpj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wblesjez.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mpsbjhul.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ijzzzeds.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wzwozjfd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rktboypy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wggpuzfu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ioryfbvx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lhssgzfz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3csrdxxdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xabnsgqf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3finypmze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmpnvrjh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nbmwphme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uqvmnjzk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3whreteid.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmomsrpf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gphsknwo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zbaslhqm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fdzlaqyj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yxlpvans.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3oavsrajk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nekzzyrk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wdreommc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hlprcjym.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3wopjvbvg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3elxtjmij.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pfplqrdb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ypmepwhp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wsckvsfz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlisybu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zzwuaprt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yuznrmpw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fbqpmggl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzzvklmb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bwzasmfs.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gsskffxo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lgsouhch.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwtrqsv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gtiircmu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3iylrxfif.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gvuzkmbh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3pnjbomwi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sqwdqmsq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cnngyabn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ovgqpgxc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rxhnxgng.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3etuqlvhe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hbxufbgc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3cjsqefva.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3suadppqz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dwbsaxqx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3pcjmxuhe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3osmgqdvl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mzlwncbo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3evwfkrby.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wqmuggnn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtreluyw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tgfiqqdt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qzeuknpf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjnxgutm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ylrvqnyo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ekpjmwrw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xejzcxgq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xtbvigkv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gousbxwv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hyufdguh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qmzxdzyb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3esifqoor.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hjzitebz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3idqnicru.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ercvktgm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3eptgnzxu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3wrpuusut.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3awihcnha.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwlnfbka.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3adlntnfj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vzpsxvat.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dtdkwxkb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gnduibak.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rcymjaji.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3auzwgjet.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ggjddhcn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hfhzitnv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3etwrwais.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jpttwioh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jfszwmnt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jbdowzgz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lygmxnij.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3revzwdfl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tslgszpn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rfeqgusg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdlmiav.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lqbygmjp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ofgyoexp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3itejidpm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxyscdo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qyqbxbzn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3alzpzjqn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lanuyrxj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ovdtyttu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3lmiifaee.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzxreir.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tlixzbzs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3yuividnj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsnlmwig.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xafbgecg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3zkpvhwha.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obnovrfo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rjspyqjb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3oxvoxgqx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ueouypik.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mfyufsic.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fzmuxjec.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xnkgkvos.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sngjgmcr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dnaqsgyw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ckgrhpko.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qncwsjol.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3udbdljvf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kswehayc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3orfrouhc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ezsizlrb.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yxhojooh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jpvlevjq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hgfozfuh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tbvopdyq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3oyoglwyy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jgrovuzr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3exvqwoql.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wmkskdji.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cyvydpdj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3aqsywkfb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3csjsznvk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ovzkojxf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bvccpefk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ukclmkpj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ahiirnur.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gkcoofnf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3glqviqad.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hqaxdjbo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jwtyxduy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aktqnsmt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jpparmty.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zdrulryj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dmqjvbun.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qejyoovy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gtrnsxvp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dhgugkar.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3guxclqdr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3trbutzhz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vwnqamcv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dgnjeian.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pgyslbpv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3msvmmdnh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bzlqngfk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qjodscro.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qbbjfczm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fdptympi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgfrbe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nsupkydi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3qeklcfbj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3txrxhkep.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ctfkqzut.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3zichfnex.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mdywpkmh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vbsznrzp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qlhjmdcg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3leplzjhm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kogxrmcs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3cjcqhcmu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rlfnyrqe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3rniszbix.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qcixpshf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3oeayamgt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vufbyluv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3likfagok.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kdhbpssl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3likguohb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3njaevmab.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ahhubyjf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qzzeplzl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xcfbqqxm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3pxazbreg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3meqepvws.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3uztdncen.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ypayducd.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rvcemrhz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xvaidmxi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fbuggwcy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tgtokwaw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wqnajuxb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocvjyrcd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bfefedqz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aklazpko.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bllvjfuu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mxokqjwf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqzafjgs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wpssfpwm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxwkeodm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kvkvipij.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3uqdhfbcu.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dmreioig.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nfiivsir.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptixzhez.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rgyfenps.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rxmdgrzh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sigfstao.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3skzyqhwy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xzhcyehv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kyssiafc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zdyhargm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xcmgotfz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3imrlfijg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3njwbfyjz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ciiauqte.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3scssvuyw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pufkvsmp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3puctboiv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uosxfydu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3whetyjmu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3chihmhwe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gtmceifw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mpxqgibu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3anuvdmtk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3viztmcpa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pcddbshd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3yqjiyttb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wsskhofi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ntfdcyri.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jwkeblxu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dhsftxxr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3hxrbqapc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pgzaobzx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uhqubakb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rcvsqqpa.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rafsxgcf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hkrinzyo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3peyzdraz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zwilrifi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gbojhvst.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nrdgbcxz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jwijkhlq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3cpxpoudh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ossxoihm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kqxwuivv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aoitwzmf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3yjctidhu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cmfbswje.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ynupplou.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ibmeulcy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lvsxkdpj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ibefbarw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlyycqih.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3gayphqyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcnflejo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rwwvplyl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tcwftqqp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3dtjfthsm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3kkfeneve.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3onzqcqpz.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dfhnmdzk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3beidaqfd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ymetrurf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hufnmskp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ugsxfrfn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hgirpkaq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3njpeznyg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3epjowous.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3wgwrfqxl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rimwlzjz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3kxgxbcxn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3omnfkcuy.html


<!-- 参考信息 -->