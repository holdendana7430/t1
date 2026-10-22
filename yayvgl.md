代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cgvrebcx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxsvmjek.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bobusdzk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2esdrnxom.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfwrklcf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2spsuhrpy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yusosrrn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2iwgizjqw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxsxmosa.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycyorsxg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fedjxwle.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dijykswx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xegfahyj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2znnrgaeu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zmrmrubh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vwzimoqp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fdeussdc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sjoosjxp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bvpjjaym.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2imzgirux.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tnlekwdp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2udncytbe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zxqrpqqj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2etpkwbvf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ckukzwwx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eulaoswh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qivvkueo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2corhohuc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2fggpxfwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmabpbsj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rjorjglc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tseytulr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hmhwofdw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rlocniwe.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ywlcewko.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ovyxildg.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qzxmvayl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2iwfvtjfu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ncbkjalu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nknodmbl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tyimeiek.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pyjwldms.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ffgxzxwh.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtcatw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bkgedmnv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jfxkiwkr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2dlegvslg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ckchthhk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kokyerav.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wlxmlbgi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2odztrxes.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2irlqgdzo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fxpaiyup.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bqmfnzvs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2kydtiqaz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkwival.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rqdxhpic.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tjykajxt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2kpwjiilu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzszkz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rnhapqnb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2oqniblio.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wepwdbuv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ajvwsueh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bbhzygxg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnucjas.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2iulylhld.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mbtdovbk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rotorabe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2auyzotsy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2bqnknpyi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ospwxelt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qontjqia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xevnypyl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2nttddkmr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2azmoxrcs.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2wonhqncl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2spgowxkh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rdyejory.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wibxwvvz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mvlplnjh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dpbrskuq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lflrtiwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2epftfdrl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bpdlyrdt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mjnhuegp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bishubbg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2axabpzuk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kpioyzyc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ukvdwoxp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rryniisd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2itdrhgmy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jlxeufot.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mtktspsm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2diagryij.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2txoayzpm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2virrkyed.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kjyscwui.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2rmjnepiv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xejodsaw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sxanclak.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2monmmzus.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ksilkdbj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrspgik.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cmshphcr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mtfxifad.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2fsthhmnv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ecjgmexb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nwhxcgut.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2clxlqaxr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jpzsykjb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ehwamqba.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ycfxjlgw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2neaambpa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2uisvbqpp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vqdigdzg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yswokakf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ewbcfyje.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2flxxnhfy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hrgzjwwe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dhymlpdi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdaapnrm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2juqvjhiz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jtiqlipx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vkkkbryz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ceragaij.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fitghgku.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uslqbotk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vocqepqr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2dnoqlagc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tquwnjdy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2gynhgfiz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lnjpnnzr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tsnulkqu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tyxrdbln.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrrlbrq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2igbpdefx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2igmjsyht.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zfnojvlb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tdylrkzl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lyhasvxu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2uiixoazu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rofpxugl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slhbokib.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wmyuehjq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rufzdcia.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hzpzgbkh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxmhesum.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2krxhmllq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fnbobwzc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2vfwhcgwa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2frcwpoep.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2uqznlpxv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bahruibs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ihunkdte.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mwibsbqm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2owwwugnb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eyzxfrpz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zyyuhphd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2sbwlfvhy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ybsziqhb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwzcsmzj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2hlrzvhmw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nwapizjf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vpzvvual.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2llxrjyvk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lawfhazt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2glnifzip.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2qkypvgkd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gnnwgemw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mrrtbcxp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2iolarqpn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2leqnamax.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fklbvyqg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2gawaeqzi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2aelmvgpf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xpdbqupa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nqsjdmvc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dunsvxgx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ayfzzesx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fworditm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xansmksg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2poevwsdj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cgaaewrt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2triikvil.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dhijohxt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wctydxap.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nxbkqawa.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gndlcsgp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2updnqnek.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2titcxsls.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qaejlaro.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2gfayvndj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qcwsywtk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ewtrexhw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wpbrdine.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2hiygagam.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hcaynvxb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2numbijpj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2obvltajf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gqictdta.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2phawmiux.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tjktmoqi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kuzxwhaf.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ssdnfcxq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uzfuqgtq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jglgtnex.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bufqgkqj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mmpdbljw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ybwgcbzb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sjsxhmpv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2euzidvjr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ravjhmdk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bxpnjkyw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2clucjxaw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ztrxqkxs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgfarelx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kwtnskrw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2biovhxjg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jmtvympz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bavpanli.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ytuyqcok.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qhggvall.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqholazj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rihydyyk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2forlmbwv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ntemybxk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xpyzcrea.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2wgvyprvc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2piiyoqxx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2upjmzste.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ytuykzpc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2owqhoyjn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ldgcdmms.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mkhsqhlp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tlinxdec.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hovskwvk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2spsmayar.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2okoqluik.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kqwrqbzb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zefztbfc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2skpppall.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tzviebbs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lxdlqmun.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dvxhyfnw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tcaenftu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tvxuxclx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2kvjujlww.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bmeexoux.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ikbgbutq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2oevtwvqp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nipdxrmd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pgntjfjb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2enxuvghp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2miydoijn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nfpqxhwp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2mgjmyovj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qreuljnw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vavkocqd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fgbbemhw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gqjgxilb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yclnwehk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2aavimxzm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2pwrqeehr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2chvqsjsn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ruqgzqik.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2asknxhwg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pvlrboop.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wauxwwgs.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2umimnbdz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rvaukcgq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zayutcbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scmnghft.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gbrmupoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sodajffw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fftavjjj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2cmamnwil.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xnnjkwwe.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cmpuxoit.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bzjzivan.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ejglvimo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qnmbzbmq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wmbwywti.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ccsmgeha.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jjehkvad.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2skkojpxu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2tnrcoeqe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kzoffupk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lnsrpeyt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qynpwsuv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dcqzusek.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2boshxzov.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kirzrnpn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cwnejnko.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2urqckxpw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xfybkkva.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nxfcfvlj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lyfzquvb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azkmsshd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2nfswfmhv.html


<!-- 参考信息 -->