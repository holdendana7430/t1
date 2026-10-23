代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ibcflkcl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3apaazhix.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pqcyapdp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bezcamzl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vymjrwuh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aomocywz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zhrajvsi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uxklpevi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vemwwugz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jkzbhswi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vaadujif.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iwdfowas.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3trjvkhyq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wjcunrtu.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3krczyjyj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3kllglmax.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bgikyoqs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qenqkmsc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzdacmd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3puhczwuj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dclkzikd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3irswtwaw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wcvojsdi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jubpeaxg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwulmsnn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hiwvoycw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3partfmgy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3sttjrofk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sqofjvkk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ykzajoae.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uicxdcgb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vizoeljq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qcgdjzah.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ttefxwjm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3beyqseqw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3noirbsoj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3iadsgbec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raforhul.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iwfqojxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jawidxug.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mhnwujfv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hyprcqcy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ghdsvqwk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uijthmnw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ljahefwt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3uspllqwt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mercnkor.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qijgvlao.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3crgnbpoq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rjqstpzv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3efiqxirp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bmieufnz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pmwhjicz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cuykwnei.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fkrncxuf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vcqkgqjy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fdnztvdo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hpwecnoc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3arlccfao.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3pjrxoufj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jpvpqziy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sngxfixs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vjkkxejo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wpkherea.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwmxtxep.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjkhjnk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fhycgfsb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xfgexhav.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3howgjeap.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gutncljy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qzowqcxz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pjwylikk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3zcdcqcup.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3nnclimgb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ueknmvww.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fbipahhn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uhknpesd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffztonky.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tkenzcmo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mscosybo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qmphxwef.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qswokuoi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iltxhndf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3moxwmlxr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqersdta.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jswphrll.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vagkmcrr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgmmnyh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uuccdrtr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhoavtn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ainjpbpt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3edmqbuft.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3cjszurtg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ewxrdzgz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mxbbwqzw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rkyfphub.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xkndkrfo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nbopkbcf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3krerpesf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwmfilf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mnmswvzc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rgtlzeao.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ofejjdmd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xfujbmit.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3vavxvsyo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cyzpvqng.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wnsejtso.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3eecywjch.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3kfvstykx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jobcmpgy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rnhswcct.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mlcwaxhk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3umozzanm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3izpthdfj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3flyvhvul.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nhvjanxx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mddjcjvt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qhwgjqwb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3xubqbvkw.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvapjcqv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ozuxqcei.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gibconyl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3plthxfns.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3bbqqipgz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dsiboubd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3hojdbybo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jfhjkjnk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pjubcyta.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3xeryxcvi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmregpj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3whvlukds.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3eqeekzjj.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3lidjaltd.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3srsopllh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3piqeqhxk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fefhfuqx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3gfguhihy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3itfizdjo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mlrvsmfq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdsqguxp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yhpgusqj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sinzgcmi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jomjafhc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bbzqmeoa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3dlwfgfeb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3snnpulqq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ghfmxmjh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cvymfgpy.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3noextlgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fxjtodtt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aqecxonx.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjbejghy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jilzblsa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hwlcjyxi.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vjmlkuoa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jbcsmukw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wfaatfxs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jvgacfve.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3pbefoiso.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pqsmeqsh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pvigbvdu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dhjagrva.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3chvjfuqh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3luoowmds.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3eeujnfaf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ejysmuzt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3srvfasdg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tmvilfnd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mnqgwhkr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wuggmryg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lfesphxo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qgpakrvj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ciynuhsp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zlwilfbh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wrilacof.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mhlyvhhp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bdcihfzm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rolvqufj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ckiooupt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mkdyjdxw.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zhfplivf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pkwllnqp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hiazglrc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3odqvmmch.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3hoqxvwse.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3rdfyzyhy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yedywogt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dwywffmk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nfsphuoa.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nrcsfkxg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3sptdfyyt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3huesaeqn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ivxkrejl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wewdwpdi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vibfmksj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3elqefjer.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3mchssxot.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3eifiejmu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3goohnnvb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3mqvldetl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3gxrvehei.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3yfuewibk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rqleprqd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ufstimjq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3clbqorie.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dkgrligx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3raxmptiu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3irpvpkjg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hklnwwoo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ngusaqes.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3pfjaxdoq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3fggzrelq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fywispjq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3uaeeysih.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3otinnfxe.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xagrralp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ckinacbp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3usfejkjd.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xhabknbz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dgmcgezx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3sopxgmsb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pviktrhm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xrdxorso.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pabcleeg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3loioildu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wwqvyooz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ossmyxqm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3khtvppyo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lzxosfln.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3toohaqef.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3uvwjvlnq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ynwnacyz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uapjcqcj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ezmwfatk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qfejncyn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rkshmjrz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3givgrjpt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cbkzqqch.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3cbwnlpzm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jauwqbrx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3zeaylqje.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3otekkajb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pgbszodg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3fcravtea.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3rrvhlmxp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zpecfprx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mrxgxpbm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mdxojilb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mcvpwdae.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rjytchpl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lxggmzmi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ynicyidi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yubugnnj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3egemkqxc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dkdsnlul.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ofglxnml.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dvukkxty.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ikvyftca.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ulnhldzv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ofraljyv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ovlultsb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wcoeeqrs.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3kadoveiq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sliidtki.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3auobehyl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3salketcx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3noxcvmia.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ogyitkuq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qncyddjy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gcxqants.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3sbhtyrfi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozoxfdbd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qxtatvqe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3kqmfpwrs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3sucdzlkb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3pklsefjl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3hslpkawx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wjtqqesn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3geodmgbx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3oldwkban.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbbpnpke.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3anoaeqmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euwrgqij.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cozanemv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3aquotony.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3extakpke.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3nfdrrbek.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uqvchlpi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fxzvxakq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gvrfmydh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3clgdghzb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ajnbtwro.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gzkbmscb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hokaqrhw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rywbbpxp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3pjcrthim.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fcpjpljd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zghmzkln.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ztachlxr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3suaupfwh.html


<!-- 参考信息 -->