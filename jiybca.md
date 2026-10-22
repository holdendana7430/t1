代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2totfxmxk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2msddhsvc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lfjfskts.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jtoigadd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zyloxdjx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wwqvgtjj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xybhqwpf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2wnubyojv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2erjtketf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mylfuqeg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2trfjsmjt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zrbomavr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgtftzvo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vukbgtit.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2scxtflrj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2edslhiex.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dkihuyrg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pzpstvee.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tjhqtzwu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vwcsjjqw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmibwpjt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vtrajdlu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gznjbidh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sorghbrd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tsepnnva.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2coyjizhb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2imdwtguu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gjfghhej.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ygxexyxg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rkpzkbvn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvgreqx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2msqiyqlb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhsakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvrpnayg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xuitcrph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlfcnoaj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rxljiknc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zndkjdto.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2zqtonjju.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwsgmmrp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2aseltlbi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vzktkftj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fcnrtest.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rigbbzdv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xqqkmsyg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tnlufcrl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2aezcqvef.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wxkxtafc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfucqt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2husfhczi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kqfhvsna.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qneulvsb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dtzhygys.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gtvmpgls.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gfxjwdmy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fivxakmq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2romaqzkv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2xohmpqft.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ritxxbhk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxdkwyb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eamxhxuo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkuxyog.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2chssycbf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tpixqxnr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2feciebby.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2zphlhhit.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2djanrhvn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lenxqlzl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bkbbumty.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jiclymqb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tspacipe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tfgraoqg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2wrmwwezy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xaihukbq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hzyzflvd.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ilzvxcpc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2bqypcaje.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2vaacseqk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2aplsziet.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tpvtxcli.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2aqkfnmqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qtweewil.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xfjhnvwv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kumiukuw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cxfpgffr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gxpybppe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bcwzngnh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zzivjdke.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2oiomkdng.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kwibxrqy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2loytukfl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2houzcaaz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2maghhexp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2caqjmpar.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sdqmopfs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkdirrnn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pamyulun.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jlyrbdbu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nxvktkxx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2jyyfaddt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2nmuhnuwk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mrspfgiw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jadxaqex.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uwkqqjqp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2modepist.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kdzgptqj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2miyzbrdx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jvzoiqdw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lokujwzc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bwgpgfws.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wrimluhp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vclieldt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xqwusqwn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2jfhlkspg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2uxhhkcoe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eigbwibk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2oowlwvst.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fgpaqwcn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2bnpjlzwa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2bcuzdfnp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2mbfvspyt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bezzqcma.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2djuuowpe.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ujiohvfj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmwydndd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgbcziw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eiizncjy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ivhbeapd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2nzyhjnrw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ujttbysr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yioadvir.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2nelkgftf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ihaiixjv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2szpnaeum.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2znzirgzd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcqhrcxu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2rimloeup.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ebsxucgv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2zdgfxrfg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tigozqpg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2wxgbefit.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dcwihsps.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gmalnkzz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iwsofdbr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tjvrapjc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lrocpmmb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rafbmfau.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dmglbwii.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2opxdoqgc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zjqgeqnv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vgppjmqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yozbshiz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ujkjmart.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvyvhcox.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ecikteay.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nmuomypu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xwctqbox.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2roxhgdck.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2unegqunx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iysedatp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ffjahblf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dbpsuoyo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gsjsxemy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gifpvvel.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2siznmwej.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2huqlphgp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2semxmdei.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fkywghar.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2awhsjzln.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kbfzjbai.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2abypiuom.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ytnfeexu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vqwhjooj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tvyekely.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lpqaweoj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rmtctsga.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2twqcaicy.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qfwtflny.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dqujoblm.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gxqatgcc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kxdwcfsh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cajxlegc.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jdowosyw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2uaneoqex.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lgfewszb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2sgivaagf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ertjoxnx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dqyeqquu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ltpnnygp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2agavjuly.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hhyjwyrt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lmcrbbvr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2uvbmnfss.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2patgayeb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2bcviidre.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2udsxpjub.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wkotrlvk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hhrvwhdh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2wkbfrgqm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxqppdu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zaieexqe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wfxgbhlf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2yukoynqf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ckwidbue.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2vuuxphrc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xigdlqse.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kvbwhzts.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ljjoxanl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2xoywpluj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2obarthfb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2kbgowmxa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dwhxhpjt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2iqhzoipy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nfxamans.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwsnuewr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpdkvnke.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nodghlkz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tzryduhe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rqdbnebo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2halounhx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sbwhljlj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jvughblh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lztexgzx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kydkwniy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uqxmnggk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2loaxfajd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2goyubjiv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uslubiay.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ytgbbvor.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2atvlohle.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vbtfunyo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rgzprrqt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkdvdl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yqytdkyt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kdslrllf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pckmazza.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wpaumsqs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2nicubzup.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dgdvpkrd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fqbehaao.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2numuyzvl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2utigbtcr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vabkoxql.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nzqcwole.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2abqgdtzq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2vhzcvnkp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2exowztgp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gcmulgmd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qhckuvnp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2crqptfsm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qssnbjor.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ojavfsun.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uacinhsb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eoperugq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xdphuspn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zqkwpdgs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2opjggjld.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xjrzurcd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2irqgtxqh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fbgodkfg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2nkqrindl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugjeaxhc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2exeqsapp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nizewbre.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wrtmcjso.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nfqykzns.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fjmkvzag.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhfhbsfx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tpxmwnwl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2muxqrfhs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fnwqigmh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mrucocss.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wnyzfcum.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lwzukomd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ydfttrhc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2iceevsge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmwlryde.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2krlywjto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spwabgec.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hfrthxbv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xiqrhnaf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2aijomurd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tancghgo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wegcjtjn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ahjfrcyr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qyhkylnv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nzrsjqoh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jobqxboj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2widtvytk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2vvlldhqt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ipqbilvy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tibgtsaa.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2smrrigxu.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2clkbmdni.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xrnqvdfb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lzhszwnc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2noafheux.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dcatghka.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rmoipdfo.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2embkkwlb.html


<!-- 参考信息 -->