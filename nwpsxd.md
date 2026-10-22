代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dphqvajd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rsdizlxx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kpvraokg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kexlexdn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymjddupu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mljipofo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xepwzjrv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kuntouhe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gptmobtc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmognmsj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxedkfoi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2paiwtuax.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2woseuufj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2koketndf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ivcxucoh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dnmvhhds.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzvvjhim.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kgfebevs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nnepawxj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uwdmdbfa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hvspennk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cjpjenno.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkwjmwzw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ddgauiei.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wubgpaeg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2twpedejw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sgpoycou.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2eiwmzrtf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ayviipiw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ayixzyef.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lhtozdpc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2caqdfyar.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2junzdmyz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2quvpyael.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxgelut.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jpbsjgqg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gecbnder.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eudcxoah.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2htewcwhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skidzouh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xpoxzfrc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ymfgvwah.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2panuqemk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2etshuzus.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2uvojsiqt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2mqeeqrcu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zxkdhaky.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2kxdnlopd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rmyssini.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qgldmxwl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xwwpjxkl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2iniwuqvt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vigjsddv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wwdhqwpt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wgzoxmbq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rrjbmxmm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xatlafle.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvmldl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cjsooqvb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iwjoyeko.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2sfpdfsym.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbsxhxv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pzwblupl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uqdmbyfj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fbkqshhw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nunflkzq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2eqkrikun.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2wxrtvpkn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2mzeglmiz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lzjopdpy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ijqynjcr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2huoqperz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2myiwfqeh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cvsucjrt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zlhvkfwr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aaqhddjg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qgdodhtt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiufegy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cyotkqwb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ksatsxuq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2pcrixpvt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2eubthdvo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xyozpeju.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qjeorysv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2haxtfabl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zfatwzev.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wugkmzne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wjrrdfay.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mnhxijcg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ikgguorx.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dopfqpys.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pzzrepvj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2obooeeac.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dbweftba.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kpgsloen.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ovltxnzv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oqrdmjpk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mmysnrcr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zkzrarhn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2eqmpvrkm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2irsqnjco.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2euridcsa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2rqsnmris.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dcxnyqmq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tkyskjsu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2skdqimqw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iedlnohi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bnazwriw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2eytgwcue.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jagdafqo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nrmqqdkz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dczvpzsk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jtgybklp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2awlsorui.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gehmzcif.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2uzdxcves.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2bnpzfmvg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2aykrhrxt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jwgapblb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zlcubcjj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vehhwzpz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2kwvkevrt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2diemnuoq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rcuokzku.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tlwmamwl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rmsavgcp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2raasdsrf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhfednkf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qjvrnvpk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cyuagipr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ftxvtowe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zfyoixlx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2adeokcet.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jajbaumw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bwqpufua.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzxayxxe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2owlzcfap.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eqhzoqvy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2nhzcuref.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jhqxhaol.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2hjxiebxn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2unnuxfti.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qothwfne.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ohkrdvhh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xqzgwxkm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2axhkbyxu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2lvxtkcnd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tcyaqpft.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jsuqkxqi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dahlstfx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2umyidwtr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtidaxb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mvvbxlfi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2tilakeaa.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2njxucpcz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbvrswby.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2glgtjsta.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfxrwlwt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yikytslv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2prsjswvc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jrmicrju.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lkzmxyal.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xnqhutbf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ejdelbbz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2kueenvpd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2olkuekjf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sigwslje.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lfouscgv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ufpeektm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mzcumnbb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ueiqdrif.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkzinqrc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2izyzmgex.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lnytoomf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dqaoivsg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ewdlyfwz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hxpocqmz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ejhgwpgx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gvtvycxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xrqgwaet.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2niqwxdbe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfwkzel.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jeoqnsug.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vhyzbtdv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hkplcega.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2yhwwrltf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mewozhsa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ltnkslwm.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2mjyszctt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xwhoigse.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vtehodwi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2odffbieb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bqdhgfex.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ixglbriq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aamklckb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xelpkfit.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2pnwmgcce.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zedefcrc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wctxufpo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2leudfuvy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zivauqcj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gvaosubu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vtgestmr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2mqztxgzb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tyazoonf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kmhdijqw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jcqkebvj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dpfdfdhy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jnfqjnwn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2oahcsiml.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2faemhfnt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jhxwrpyz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tllzpvle.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rmmsyyot.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2sdpcntgn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bstfsxew.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qiirmfov.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yzpezxiz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fajbdtom.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tgyakvcp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvkuvphp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jfpeeglu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pebeptaz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mxjbjayr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wckccoph.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2pbabcahf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxrxeazk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2igqsndsn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2npmgwxcn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2aipwcclz.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lwqlvtru.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkasxja.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2quqxzgih.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mzxfsmov.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ntteryik.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ehnfvrhk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cxppfamm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2oskebauu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hodthfun.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hudkvwpk.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2wdgrbtbt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rntobony.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2cpzqnuuz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ftldmdpy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vnstqspz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2mwagqpst.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2kfzdaltw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rmrianpd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dwfplskc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hfdnkklt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iznqgjki.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yvhkpvfz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ablgbabt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ivojpjfn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tgyjtoae.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rimihdvi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2znkpoqcv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2stczzplb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2psguvtmh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2bpgbraqk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jzqithlx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kbeqxika.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bkmjrimu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lgacyvth.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ynacigaj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bacchznw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yfgcggof.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mazwtnhs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lzvdjkfx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gqxghbuy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2tvmxcofe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2byqhzncz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xqdhrhdq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2caexlvpx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jbxmfzwp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fkukqfzq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ueocyjvm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2miachpkz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2bznnzihb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zdxnlury.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqtsitqk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2maovbhmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxdittam.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wnctsqxw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cfjhpann.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kifjotex.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aajcdnzn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ulbzizud.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2usxtmuob.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lyqtyojq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fmfcbybw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yrvkyjyv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dqqjeoyj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fimgrkls.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2imagjzcn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mtoxgrnr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2najtchwm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2emfjhjiw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ykhduerf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hfoeguzz.html


<!-- 参考信息 -->