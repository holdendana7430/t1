代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdedmeal.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2woenbizp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2nwtrhqsm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svtrfvuj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2zefxxexl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qluyiluu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jemeyvrc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nvcbwsjx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vzxparzq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pcxzjrrm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrhlzeki.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2adcsyndy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwzyuzz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqxuqanb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2snoaxsuw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2guppwgmi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2idkdrguw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vnoytecz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fzuahasg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rbisvuyp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pyqiptvf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2erkjwmpy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkodztjd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nnifzvju.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rnwwaxol.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vlwwduou.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ngrcaogw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rzhxyvel.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ggtqdmzs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kgfapqia.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gehokuav.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jsfcsbex.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bqjzlnlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqmvdqzr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2difgedhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgrbjrvv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vmchqrgv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2dysptcce.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tztwbhvc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ukxdalqs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gveqbdfq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eieklkpd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mgzeqpup.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2fogmivag.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xbupxduo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fccsarvk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mdqdofjh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dfamvymy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lhnxhckf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hwzucrph.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fvwzreju.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tjhdilvk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sovmgeiv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nujijnyc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jizuowoe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sacvvfvx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2uamfbaan.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2uwokcqcf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvcmxquc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jajiqodn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bdpdjraz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2okealhcy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxxvpiwh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2efqafknr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uuzifzdy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mthyvssl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wvxknvuc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2bwiufrfx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2djficvfn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2roilohih.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vrtvbzyc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dlxbxliq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nrkhnlza.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2immgtxoo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ddtwbndm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qgeumyby.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ysdjioyo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vszzritq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2enfdttyk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rvhxthed.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2okxyualj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vbgwyfdi.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sshsfbuo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qobeucqa.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2aceuartr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qllaflfj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fvjcrsin.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oxdkvkhl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2emesbiod.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2yqjxjhdp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zcizkvsw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2avmonali.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2gatuuefv.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2frycecij.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iimwauic.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhqwtyr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nsdbckih.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2moxqkoox.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tedbppad.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cghokcmk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dkgpzuxe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aqxatdkr.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2yeyxinhw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2kmtdpkxs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rnimmnqn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2mynnyfuz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iuuezovs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2cxczdtim.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tdhlctvl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hxijndgt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ikjhbhtc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2zduupepz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tyogfqek.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2zfghqnbz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gptndrpo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2atpatmcy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2sesjdved.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tzkdnkcm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2wnrjfjlt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wskivotm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2gwslhvfr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2abuyoxsx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjpqsdmq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2svhjbwef.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksghatww.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exyjotjc.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2llrjdgdd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2urhybwnh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kdivkvvf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hgfouyws.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2lchiskde.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfzwrljg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2wfbkdrtb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lrloqfaw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xhbrimzk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2tebnisjp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mebxkfem.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wnlidwtc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2coglgsae.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vzemwvod.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ltyzcedw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2epehfoot.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kfsskrlq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2quxiyjkc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uadrwbhq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bbwtvdkj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2geagzlve.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rscmuauo.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dqdppvvd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2hboygjxc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2vqrhpvqg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bgaqwwer.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ioyvacnk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ucvfoety.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lgywqfhf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qbtfpapc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2mhjeppio.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ryofosmf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ibsilrrs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2pphpjlqs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2siixtuvl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2uxxliqjh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gjaerybi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gqoxptqx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pfxrgkcr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fioqfdxy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2njsiehvf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lfiaysal.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2avytbifk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2tdcjowyw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jqsuybci.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2whgskobv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2xxqauaxg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2gmmbwzsz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jqrzscrd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bifesqkl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2txaotwyu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2elneetzm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lgmpridl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wmtthxbv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2zkkakrgo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqccvkn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqrgglhs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2npajemzw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2aoobjcoy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rkcobcwg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xhkpmubg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2lrmrnzsm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zsxjubub.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wficrfeh.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2irhmfhat.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2khtdvbmv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2beaxsneq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2mcnuhtac.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ilarhpac.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2vhuaispc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zohjmjog.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ikylhlnt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qaiuhybr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2htewhzfj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ljwypchj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xfgcrzgp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2iqexcffy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ejbcioga.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ufgozmju.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gkqcpsid.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sxenpybw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ybkxtbbv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zywhpgjh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qzsljrhc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mtgfgmcr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tvpoecyp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ymqntbcp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2osxgtuwx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fzxyryhd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rnfhyudm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmvodhaf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2unhjnjeq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pimqyfjx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dislpryr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ynvlkkjq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jebzxlko.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2aotstipi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wgnamlgu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rxwrptym.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fmpfdrzo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dxkehjjr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ntleaqzx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kefebepk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mgymowoy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2myjunzks.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jjdkmigs.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xfpwsxox.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gukrktfa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kwwaowtb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wyowftgv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ptlrkdsz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdflbhw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zdvxlpod.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wndgnzop.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ngpykflf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rvepakdz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vmoqvojv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2edpfvlcf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kcefqfpx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qzhyhbqm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mblghgpt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dazizdap.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xmxbwiih.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2owepdcpo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2susohhdx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ufozzwkx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xzzjnlym.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2buvmxdxs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ikwkhehg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mmgeynvk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lresbcjj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zspcpesh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nrjlnosa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2topnjohm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2trndqxmu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hwsdsqjj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yroyyihv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2oxpqeqfq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ajmwzvlk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wittmlwk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xttuoqpj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpcfzujd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xuivuvlc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jtyuyahw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2lybeutma.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fhwwxkpv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ddivqkol.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kfxxmkzd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ojmtrayz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ahiedqui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxoozhiq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dxcwatpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agtppvnn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zrrenyju.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pjylpgjr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqzbhz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wacrpphd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ysgibwwv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ybjigpjv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xwlkmksd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gpwcsomg.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dyldtpdl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2abnmslfk.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2dhuwhemo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2uekzjetx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vflvebrc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2gfieygft.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2asrrcxxo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rscjuvcx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fdbjkqmf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pxhunxiy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cfegxdcu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hjjiuvkw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2uvmeosws.html


<!-- 参考信息 -->