代发 wailian999

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gvmgislpe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/galawtxnc.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gfgwhyugt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gurjlxylh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtzmevihy.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gmagsskxp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/glkrtxtlv.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gpamujtzk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gnpbzedqd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gznwkcxkd.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjtogeaql.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gznpfbypb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/guavkihlc.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gneixlbaa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqswllacc.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gpjyvpnmr.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gfzyzdwht.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsmqvijdz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/glbybcloz.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gpphhlksz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gxzlnyfas.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvgdfqwoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gzbnnffds.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gncrjqymt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gujzmdyqq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/godyfpurw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/guyzjvxbv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyqdesuna.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gwuplbupa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gjagrqxrd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/glqxatxwv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gjvivxrfq.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gupdebdpj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gljymbhym.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/grbbroyrd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gxxxwjull.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/giazedlzw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gxpioakuy.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/ggzztfbhc.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ghyffjfkx.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gjnohdwfr.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gsybhjwcq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gftsjspww.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gzecigyse.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gitxjoqix.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gaaqmclun.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gsknnvrty.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gnjlirtwf.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gbayzkkki.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gqvanqgqg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gwhmmdqzy.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gwouuevln.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/ggpcwucba.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gyhyxsbfe.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gjvcdmisk.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gymvtozzj.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gtddscmio.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gtytenebi.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gowoslujh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkjxnah.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gokndsgbl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gynmqqpld.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gsugfizvu.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/glxcxtvzc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/ghecifbhg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gsnyialgj.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gpgrxlzcz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gofcmhevd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gwxhprekp.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/geyqnwcxp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/ggmzqtapi.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gcssgxyzw.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/ghqfkpban.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gxupdvvof.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gufrnylyv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gfstbjstl.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gqbuhsqzz.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/goekhlrbn.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gixntsyfi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gdqjbylel.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gkjvcnwkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gyyjqhprh.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gfqspvtdz.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gbdbuxdnp.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gaecgftaa.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gvfmbjrpv.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/geeucftlq.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxykfjnoq.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gxehakije.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/guqhdokpn.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gwjpsapdk.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/geinvdzdw.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gkzrmzary.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/ghdtoslha.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gatnfaehn.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gexcrfdxw.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gsqezwozw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/glxlmtqxh.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gsuxtdjlk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gvhvikksz.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gtdfahxiq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gjlajbvns.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gwhxreghi.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/guajwavsm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/ghkrjqpaw.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gljzskpmu.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gemodycaw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gjibqzjic.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/grxbgpzop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gbzlxyfnk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gotokkcwg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/guqhxyjeh.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gqpewtdnc.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gqmfjiwtb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gnmywlumi.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gsyhbechj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gchnmesvo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/guhnritdn.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gtxxtmjbo.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gkabtjiys.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gpcscmsyt.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/ghglqxkwe.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gudbsvgnu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gvtemjtbp.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gwonaeshu.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gnjnfrbrd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/glnoghqzv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gkzmbiqlk.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/glwetmgda.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gwjrwzjjs.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gzcqyfbli.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gqznikyjj.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gjamwopyl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gymgratah.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gsekyoyti.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/giibynuqt.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gviezmnua.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gecbmpujn.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gvldsvfnh.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gmqmlpfyr.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gofsbasjk.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gulccgzzg.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gwvewzayc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gsndwehcu.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gxtdeqysr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/guqiiebat.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gbddcyaea.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gagzizchr.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gwaxktxxa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gbwnzyzmm.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmybelwpv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gbyfnfops.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gpmpeafpd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gdwqxasbd.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gxhjmqkwz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gxheuvzko.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/ggjsgxukj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gojykpybt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gktjtukdw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/ghmgxzaay.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gpeyvkztw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gawyplfee.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gejwxoeqa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gwixrllqy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gbizzoblh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkiyvya.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gjmyifqkh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gupcgfmjg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gojwbrqxd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gbgeztujd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gqbvchcyk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gsmjodses.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gmncffmzw.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/glbswjhvq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gvbisctwn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gyrjghrtx.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gblemapbd.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/godqafkac.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gcfhvfglf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gajvivzca.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gnbmrqcli.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gwrnekagx.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gwxehoqir.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gqcmmqdef.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gqcaeaibh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gtijwssbk.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/giunlvapx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjjdlnjxp.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gejtrxegg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gaymizgiz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/guvhqhnwg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gypcjojpk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gvlggahpz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gzohdeazz.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gpjrtdyga.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gdghqktsn.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gyrdbchqw.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gihspoaqz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gykaqcolw.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/ghlmyfynu.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gndvbpcpc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gpmmnsvvc.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/giywyjdwe.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/ghjnzmqhj.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/ginvtqkta.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gmlyhmomd.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gpizcdcud.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gyvipwvql.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gheypkwqr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/glrwulgzc.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gnlwpdpuu.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ghhyjiyre.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gvxlslcgr.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gujpwkrxw.sHtML

[U94] JS：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ghdnmlcvi.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gcfliksbi.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gpgwcvhxc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/grzeatqeb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gormeltgq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gmkrzpqje.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gxtbzalop.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghkyzbgig.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gfhvfoldi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gdmwwbeux.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gdfiyeuqr.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gedibyrpa.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gcgpvjsfr.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwhcrsuct.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/grddfqaef.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gktartshl.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gjuhxnsux.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gfosiobyk.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gjijofmxg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gbcaxhfsg.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/ghtjsjpcj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxiewknua.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gcyuduslq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grelpdeam.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gagkhcjrz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gzalsvebf.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gizzlmcvv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gnkrcfidz.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gkxygbrag.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gjgcqbpjr.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gtwafsset.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gskpxddcu.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/geepkncjv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gpitjjbth.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gnwgfnhqe.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gidtbqsvg.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gafwsxjrl.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkxslscrk.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gtzakduhk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/griiipvlo.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gvzvlyarz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gwvqjlvmd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gheibcgwq.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gwkilrmkd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gzqjkwcki.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gehnpwzft.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/geipgagwq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gptcfvgeq.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gsbxiidtb.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/getuihawj.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/glircghhm.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gjzmuogdf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gmzftkqbs.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/ggtbnyhzg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghnrqxpnh.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gdlbuswln.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxlgojcwt.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gasyguabp.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gfkhgreui.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/geflsrffz.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gwuijwcwc.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggycwxfie.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grdtgysei.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/grndyrzdw.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gimzormxh.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gifqleppf.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gjfkeskwz.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gipcipnkz.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gwwjnfjdh.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gsxcwqfym.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gzwyxzbpe.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gvkhizirn.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gnymwukwg.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gacxhieeh.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gjxmorzcm.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gqdubqlye.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gedczqaqj.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/ghbokxifw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gajldgflb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gevkjwhxn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gwompnpal.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/ggljcsmct.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/giksiuccl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/ggerqqccb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grexhtbta.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gmyrajxzr.sHtML


<!-- 参考信息 -->