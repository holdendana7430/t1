代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kavpcuft.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cdhqnklh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gfrrzkhm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jvdpbyjx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hczzdbtl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2thxlbhur.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2oojjroeo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sulzitba.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gqdjqbft.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sxefrqxx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucgrnddf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wpilgvik.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wzckikbx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipcpoftw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fbbpfhls.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lobwoodo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2nzjwjkgb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqinuonc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2eabmspjo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pochzjsz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjdxyymk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjiomnw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcupcjpq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2yvzwxrww.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2bnzqbxii.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bgqqtwgr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2whmtzulh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jighcjtp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqlxjd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zaxayedx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2llvjzaec.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ribuzdmv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oembrzde.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kfcuhqup.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxlbhsm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mahvitui.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dkhvvrnx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kqhfzpks.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ptoefrez.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jyedemzb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gcmbqotm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zlmwrnqu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmvshc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2eeixrwhu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ppiypqgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntjjuyie.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2faxcqtzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfppwhem.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nqupoocg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bmqganws.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mqecewso.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kgjgqhqh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ktzbqmmx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wsvaurtk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jeijqpyl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2tmutjbvy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2aevghexj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tidjrphd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hcvlozfz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vgouhsxs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uaowehal.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ypgggjyc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2occqgejf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fnpukyyf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yolxalrv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2krpzbxfj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tadpacow.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vxkdncri.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qiqcyjxz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lwockplj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2votumafu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpunouc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cqcwjhto.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jbnnzxij.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wnvquqji.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uebuvfug.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wmbifwwu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jghvsgzq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2thpkotwj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pwpsielt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hurueori.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2evhulbbo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2zaqwuske.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fjvwlgvh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ypugmngc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdnjysdg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cxvrdrkv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2rnmwovyl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2nczjuvpy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2juxbazuv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2paaghixq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tjogjdgk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gagsisgh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2paiejfyk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fymzcvpj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rkuazrjj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fhafhzml.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2rltvdsug.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gptzzvnd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2kqppsery.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jdeosdyq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ybrpummm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xkhsbkcb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2supfmnsq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2sjdogcwm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2eychgjie.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2reijrsyq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rygvrqot.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kqpmyxae.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nytjtibj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vcfdtsze.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dgnznsqw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2khdkmzud.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2fkoiqgyt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2uqkakmxw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pifwjdyj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kvqgbavk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2fnmgdklo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ppggfxft.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jefcablq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2frnhxlzb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2byooolog.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2djxfkhmw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yjjfwnlx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jioehsyz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vxvimkwk.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vdrsddiu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2elwdzhkg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cjqowduj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2mjkugnfo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vwzmhlsh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gplfwcit.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iqigjzpi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ihqejecf.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aaamnykv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwdwcnob.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2edzrygmk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uitwwpxd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2beiajudw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xbazzota.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2uqjnpwkm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jcjbulmp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ikmqrcym.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wbbpveje.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kvkvnomd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ooknsrbi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cfcgzdcg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mxyjuczn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kspldqme.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2bhwzctel.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsjezgli.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2szjbhkba.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2akingxxg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nwfewohh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2czvfdliu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2sxgmwesd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ljqwrnsg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hwikzrqs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2lkrrnmlt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2leqssinc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2awpshndn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yewefjio.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xzxchhfd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dcigwzrj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qszrudie.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2furneobo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qfyvrkmh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uuwjdjwk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rpqsgojc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddcgwzyy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2guemtktx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2guujqsaw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qgeyxqfy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vjouuoai.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wizfvgqj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cdqwqhgf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ckhnylpo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2isxprwun.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2lujerobf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hfixfeui.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2oxgwrkeu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2pbfgjvao.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2lljwaetk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2jxzqzayt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bduhhfnw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnipnxm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xklpcukh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2zhpqwfrg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nupkbffk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tharmzqx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2nyvnweoe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zwqtujkl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rrdqydot.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yqolmtsh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aqxpsnnf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wfaevqif.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qewiygmb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wgteioav.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tvbijkbj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rnsoluls.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ukgwlbpm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dqhxjkfz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2idztefvz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mvalaflx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ekjrbnif.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2jwpeycqd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rooupewg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2kuagdhyc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vigqxdit.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rdcgydee.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kffowjsz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fbcfpuag.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2qftagmbw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mlevtwdg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jogwismp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2yquuxljo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2syuqmwdj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ncmihzmk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ovjydaul.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2svwbokkl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ldopsinx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pbprrlal.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cfremnvq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hhyyfvhz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2sblwchdm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2habsdzjj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fjnhqomi.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dyrugidp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ifnemehf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2strhegea.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2keseozjb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlorgttj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xoqrgfbt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2omeghlje.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xqahghes.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nbvweeeq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2bbseefhf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jhuajapf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cgaawfts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nidcihjg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nfvwidtx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2utuhxkgx.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2tiiqtxsv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ulxwxqfv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2muesooqp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lgouqxfv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vocqyqgl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2rquhwoxu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mqunrcal.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2djphohii.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2osoqjfsf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xifcttuj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wlyiidwq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bzdrtblz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2htpnhdrk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rwbzausf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2chqgdovw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qdvwijln.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ktgzzwne.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fotivuky.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tqohukgp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2goltqhpg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2eapebjwj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bwrklksv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2igzyoiko.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2wqstsogf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2akjnpnlb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dxqusklt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xwdsdufk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jjxtrbft.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tchwyhik.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2owgbcmnl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2aswcjjnq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pzjfplip.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2crtdefqb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ztnbujpc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2azdtvqgw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jzkhanij.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rrqukwry.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbxpaiab.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2mdbuvfdf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kkxurmuf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vzhgkjcw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2btqvtonh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rqvugewr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2fvczdnio.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rzludagt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2owyynkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fycnytou.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ykxjsvbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fluaiewp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xhkgzhxj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mhbyelje.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fbvmaoqk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2erncrhhf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jiwwrjig.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cvjgebqq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zetunhzf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bjdluwxe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jtglcrqg.html


<!-- 参考信息 -->