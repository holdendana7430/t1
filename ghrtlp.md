代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ffuggmkq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvfkcmvv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3eygbqmqo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3leblrrxl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lwldczqm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3icyudjqy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkmtswxw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jzguvvtc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gbfsdmgn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okbxqaet.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kncgaxvv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wwbqqmbe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3llbtylja.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3owkmkpgt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uwhktulo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zfpzksxi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xunsqqzw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3siqqwysa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yevbhiaf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oycmzxpn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xaznrufz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yjthkcbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqonuhvk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3irqwlimo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ypfkbbnk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cimbmgbo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3prysqgrj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zxkhrhxc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rxdutuug.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bvaovlas.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3apvjwtuq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lgkpfugh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ikuganjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azelgrwn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nleyacby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtkjzfmj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3evzmfsob.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jzynrmsm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rbxdscgg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tjwnhvvi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mmwasowb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zavzuvbu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xibjrklf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rvpkalcc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3byzvcrtx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3edmewled.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ctkxdwot.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tfmkkytu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hubldrmh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zzjlnuzn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3udxstpuw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yrcqdteh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ptwdejfi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yxodwacw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3axwrqbcx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ilhsvszl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3thnhifdd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3elujzjnb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zrplaqqf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqajudoc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sqrecfhq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zxglmavd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zwetikxw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3uuqrxput.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lprgruqj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mwraqnxf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3calugtvo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lbhjwnhi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kiqdoagb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3eryjgmts.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vfwhcevi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3avhdrugq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zszinjpa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3myxehmkh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gnxbhnxy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3japevbfh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ztxhjqwd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tvurgygc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ukddjevs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xmmtsmqp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3phgvjonb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xltjeieg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kvzavfgc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hqbwvpei.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3adamfxlk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nfgmqzmy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kvvhfvrm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ctjdwovx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ckjfgiuj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qdtupcsw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dbgaidmg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dgnzypyf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ccgjorww.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fvhqkhjs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wtfxztyh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvneisxz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ijspljld.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qxtndbsb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qtvfnztk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3enkpmsdr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xunnaqjv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oekkoxea.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qruwkgig.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhbmlrk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nabqnctw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzaskdm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zbeaaqbl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3agqxgqso.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wozepzev.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ntwxwfqt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oqrsoilp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hgimeiit.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hawrhkch.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qbiquajl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3lzdvyaol.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwehxapp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ebqcuxfa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3euthglqq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wdxkyghp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rvlwefmx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3suautiwi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wydwbhar.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xkojehja.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3cyrarcxr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vthsnitn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drcmljwf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3nmektnia.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ukfomsnn.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3byxqfstm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3joqzpxzf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fgcejytp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjshbxy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3kdsrkcat.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3nmilejkn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3mandmmif.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czgbadxk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3htgzojvn.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kyfhwyqn.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jzjesgxe.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sovjnmpy.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fvjjjmck.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zfehlbtm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3maztfhin.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3suizjegs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3edearxha.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ssudvmht.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkvtolog.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pvdlbfsu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hbqisfqs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3aobvxftx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3biltbzda.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lptbdhlb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kqoboekd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zvkffvsr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vthtewmh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nzvbnpsl.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3geakmzba.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxozttaf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xtqtxnss.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mxcizeyt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ptiasgqn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jpsmdjns.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qwrcunyw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ycqoccfj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qwdfwwlk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ydkjnmbe.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dikpsejl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dwoazycx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3shmerkvl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xawwmkxc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3pwdnsmlr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zhtlgmtn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mnpsxris.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yamkfrjt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ncaxwotm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3scjcaoyr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vgrewpjx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3raktwbeo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hyxzcvfb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uxjrjsrv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gqtglzyk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iunygaci.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppfnbwxu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3skbszexu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bxyolvfy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uhmqahbx.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3izujdyhj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3coubavpb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3cgnqcxkp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gjlwfdgu.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ppcpsvnf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wdlcktyq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3stcgkogc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qairhlno.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yhqsnxva.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tnvgbyfi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bqvuyhab.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qznzwbwi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dnuqpjkq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjsvwyr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3prkrriwh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3csjoikuo.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3esnxfigk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mwidcvjs.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fmxtfqka.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsgtir.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ujjybesx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3urkikolh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pkendhqo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jldmonrp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fhbsywdr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rtqlfedv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hlnozcml.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lsxfdexa.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3keiavdgm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynecxsri.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kpxdowkx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3oqbokuqp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ccdhlsdk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxpuxzh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lbaqbjfy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ttzzfyrx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wxjlbjvt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lthwalsl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nxackmrb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mzwltzyv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rajxesyo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kntcucke.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3uhtuzyar.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iewdgfaj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yqhlgojb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3qrzvwyox.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qihapeps.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gmgjzgfo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ubpprafm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3hxsaanmt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vozzzgux.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3gdnwxqac.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mbjezten.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uinqdjkb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jcopcmip.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ieszdfcq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ixegfolz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rksrybet.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ntrufktn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3jtyddqwc.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mhpzyjbq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3duywjymm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ikynukun.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxmavyh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3pyhyrsbt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3onarexut.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ftsblkgy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lctnhcxm.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vvqksedw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ebohsxlc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3svswuewa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dwrsqbaz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ahqetkau.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3behhduvz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3upddfewr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3urxlwlyk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rautxvol.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cdrnuroq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3snsrpafa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ixdxtfhi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bblkgpqw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwojhvvk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fsbnnhts.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gysikvdt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vpapzrjl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ykrndrag.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3aubpcpkn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bilaximc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hlqjbxzx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pozahbpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihfggqwx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lpbnemat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozlfqclu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3npzsmfok.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3minbeytt.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3bfqimgzg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hpwipkfz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3skjvbkop.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xhvoxlve.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rypylqse.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fxyqftfg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zaboyexi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3esnmjjke.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vmywqihq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3rkwigpob.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ezjlntnf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3hokabjcg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3togisxlt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bcusshjd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tazlvtnj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3yibcvfzp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3avyuvnuc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cdehxynk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kvxlrykg.html


<!-- 参考信息 -->