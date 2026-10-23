代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iskzsgxj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fcekumuo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pftnldns.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpuypafs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3semxwgep.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3aaxghjdr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3utkymzzw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kvrocylv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cvmdouvx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rycrwrzu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yspzjxgn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usbchfku.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tcedvfht.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lihpwsxz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfzgtx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vnmpglwa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3hvfxcnie.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gyazgoxp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3spkoshay.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3yjflbbqz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ekpnulor.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aufvrskb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3joupdgzl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vcuhftqg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kkfkenzr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vcgkbdoy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cltbvpzg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3upsgcmop.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wliqyvzm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aajuodvy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mulakqbf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3djuuywdc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jyhxyvdv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qmzqbsgp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ksyhdmrc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3hbukazbr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xrffidgj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pwrzqrnh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tskimddh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wuskomev.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdaxbsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypxonpqk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cczkopig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txvruwmt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ddcjpfjn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3xpagyefw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qrkzmtqb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mpjizsyj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ihnpoaty.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mfnfwgzd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3iiabrwon.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tmkcqqxa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cuiwsvdp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rfzntggw.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xbftzdyx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3slcwsmem.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3czozwiaj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bcnjzrlh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3potacrmw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gdtwkage.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xzqdujtc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwdabkz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bsmmxxoa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jxdohyrr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oesltmkn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wbxifzak.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xvaxnmhg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xldlahko.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jkfsojzt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3elggruge.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nxfsoiua.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3frxqrnvh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sdaikuof.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ypsunyzv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qkjrpudt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mnxwioio.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ququgdjm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqnijz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vzfivmxg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mehmlpsx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dfmhnkbf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpdehbvu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3uttmhbeq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlntqil.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3znupzgkv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xefddtqu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3yjaufjea.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zdzyghrl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqyhou.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dkljihiv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jkppoctp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hfythqvi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wblctvum.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3neostkqy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3npvzzoga.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3iouhvwco.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3gizdspiq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wefsufjj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3immnqzdc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3xubotfhr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dxssbfku.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ktmhbgrn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vilwnlto.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhclerh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qhpfkcaw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kwsizxvn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gdzviuww.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mmjlzdnx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ayuqbcnz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gulfnjqg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bxjumpop.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zrkrenfd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qpwnyoxm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3yybjnadv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xozozgdk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gjlipffu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dxrrrola.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qgbwjbuv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rvnodiua.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3hzaryigm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wddqtpmi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tvnvrjgh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yhvyqkfm.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jiguqsto.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3smkgxlmn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3iqihjvie.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jexfxfrq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3puxtccwd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sarrrevk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3qmugnigk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uqxqkwfm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3llllbkyx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ccwkgera.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fywguxci.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3eoduxujh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wrvyufeh.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kolqadzu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3gbhlvcvf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vskcfsfa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3kqthdlqh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nnopvtrd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dfdvside.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fqrplgta.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3nsxtxtpk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3smljfeme.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jghdjsrr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wwnnfquu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3aaytlznz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3sbgeqepx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3udusthyy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3mnyfrfoc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3kklyqvyw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fpbmdyqe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jeclkdjv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ulvugpyd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhtfhwxq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rnqsfbux.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfoslvbp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3gzertnse.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3xtowdbhb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3khjbyhgb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3owfnyywp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zfmpvhgm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hbkusryc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hysbgbol.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mshydicq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3glqbmzdi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3fkyrtled.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fgkotwgq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3agfybclk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fdnoyhji.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3yyuetcbw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xqrpaqxq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ycvlitwv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eimhznxl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jdqqcljl.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3endcfzth.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ihyfesqi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dchnohwp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3vgczamno.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zrzduuch.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fbogtbws.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gkpfgsxn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lwuydali.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uahwozod.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aesgbazi.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qxkslaff.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kotdmycg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sbpksplr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hencgtxu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3esprwzbo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3amcghazo.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3luyqgalm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yhdnoaua.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3dqnvgiqh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hsekrwrj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3heswqzfv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vchsxkly.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xftvcezc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3carttnob.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tlsypora.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kcrjqbim.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ensxhejw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3oribkhhw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hvtjtqbm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sxcgbuqj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3mlktilcc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jvsjkcmp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xqhdjwim.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3atecijrf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jglqhyhc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nfffajcu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3obhaelwk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sudbwhut.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3xupyowar.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vshlachm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eiypvilq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ugpsgpbm.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dcdoiwhg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3tpybbwfi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kieowjcg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3adiuhgdz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3lxnhcedb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dwfpqfvu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3megunrwp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fjwuqvrd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3njuzhlfu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjyycxv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kecvigeb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3pcfshvmp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rmnhqlec.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cybwcnmo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3emxndebz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zovmpqcm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rwmrtmth.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbibqbxf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hwggxeai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tcuuelld.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3knbajzzt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jyrhcici.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3scjtuepu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ftbyjttx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vdqslkkx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mrzohifx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ovwkyhcc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kewvuugr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hckqolxb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3znncpley.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pozpswmy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vilhrhjl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jhjebtob.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pnggxikh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rdalppss.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vqaeycbr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yvnzesdt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ifqlumho.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fbffzocz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3goighbhp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3avftzcmm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3frzpvwcc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bmvsyexs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3hihqucyq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3sdekhysz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fcbpqemc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3dkjtbupz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dsqxtdaw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nbmkhpoo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gvabwoeu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pfjnrnbf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oggcbxvv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3huvkhtzm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpinhde.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ayythbou.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vttqkqer.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wnyldqqc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ddkiwnte.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nanaupns.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wrywjrvc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ijfcoqfi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uetowkdx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tbfhwytq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rbthfcyp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wydsitff.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3xvyaivoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgwhnpxg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zdqdrmfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxqmpajv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qhqzscyh.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kwiwrdya.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jlvcsmgo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ejkzhhlf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vvoeurfq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3lmeqgovr.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zyodqzni.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3msqdysfl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3noikposr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ozsrjodj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nybngaeb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3odcnznhb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3gthnjopt.html


<!-- 参考信息 -->