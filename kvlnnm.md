代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qpptkhss.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2blxjmwgg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rnrannar.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rnwvrhxo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2owdfqmws.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vzfskxkh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2wxtoyoga.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ohuhhway.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oaybsxyq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mraxvkdd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlspkncs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wrozpnaf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iloypqjp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ywlxbawc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fnkvlddi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoqlzayo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2qhkmrvlf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ukgupnin.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jvwekxzk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omzkysvf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yogldemt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2thaqumhr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mutwhzmi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nkivfdnq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2twrtajnw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vblciebf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2djgtdldl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lzechbbh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hskpuljy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2flhqzzuq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lutduivr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bomztrri.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsvhmhin.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uqlslyge.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rsywedvy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bxgubbff.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exuscaot.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rclgmfbm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyqwffk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hqxwewwq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lzvdgbxn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sfoozcoz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ebsqcbzd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wngszqea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gsieauvz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wqtjwmrr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yjkypkmm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vjtylnie.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2himkdsyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyzckwac.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zaayklug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziqsrhdc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qvqaulhc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qxlgoqxp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2iwjvnssk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2duhywtra.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jspnyhwb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ebhlcnlo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2newlnqwm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2xpyxxyep.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hakdimwz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cuqwzimt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2obumbhgu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2srdhzrfi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pyrhafqv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2osugxtxx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ozygrojy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qhfpcuvh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pgiholia.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2okgyfwmh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xrzmyiyj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2srfnvnmt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lxfmsvhk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lmlexkcc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2liywmspe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2diklldkj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydklkjpe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ytpwamwy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qkhlezau.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gtrxones.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cdhoiwso.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2youtmqok.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2pmouwyzz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cpwqrjtu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jnkyuseb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2jwvfdbls.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2swlckytb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oucllkyr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2haeephsb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oeswykhk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2tkopklad.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zhsmlxpc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2srjkjgtp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qozqvddx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ptshmrjl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dwyqpqeo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2zawdlexx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2oyizapqx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2uaxthrme.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kpgoosyp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2efjolyog.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hantotqi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2mfdvrzlv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmxtjwx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2frvbugmx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xfmchlmy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2xkhbxfmy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2nnggygox.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wbrfnqob.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zmizgfor.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ignnjywy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2shmnomld.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2utqqowek.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ttaxvxgv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2farvqndy.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bfwofmkh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hhtiwjkv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qhpgvwyt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2phseafsm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pgnoauce.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2hewstntj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ayipezym.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2yqnmsqtc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2woeurcat.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zqyjuruj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2awqemkqu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hsumpvpa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ogyopxiq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2tnkkpqiv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jsxbopgw.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vtybfgxu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eqrjggkp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gpbmxada.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2rhprprys.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rjvsoyeu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvepepl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hxtfxebb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cqhmerzh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbquamfa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzibgcgi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2srljqzlu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaaudajq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dmltgihw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xjjcpokx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2riukhrvr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2jtazynil.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nfpocflv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fholfwdi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2weeuoaze.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gacgasaq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qihhpbeg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2orjuletp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wazfuazi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rzmusatu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hhusbrmd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2savjepqk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lewftpjj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zowyaetv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vsswqqwb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2nyhrbvtu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hjgbxdbr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mnugaifz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnmmoabm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpczzzyy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2owqlgbyy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgapuevz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vikbbcwx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2uorbirqs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ospltecc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pqpyydhy.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2uezyuivs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yweggskz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2skxrvffc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zzbdpmso.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2aejjspkh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bbabzbbf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dkienfgy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2udsmoves.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hmhcmsjo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2loiofsce.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pgdxjhdv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rudcknfd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2olxxjgpv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dhjzrmly.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xnxmilrd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dxnehyus.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fyqwgnub.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2azvqehpv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2miycqmhu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfdhxhu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2fgzvbubc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ihmwkcwe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zibncezg.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2fqoeynww.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2uedyhpta.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ghizvpzj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yyypdrde.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pvuieegc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sinertgg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2cajamrwf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2cotlwmbf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ajnfyham.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fypbjtdo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2pkkosrco.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zazelaiv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hfetfkgk.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oaeirrij.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nfgpaaif.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2jynzrkkl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jjspickk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2celaroxn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2utmhwdza.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xkdbrmwx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lezkzhln.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2llzuxvik.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfmuuxq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ryqrpncp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fnejaeyy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2glodrrjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2stvxtskv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ukpyzzcg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ookmojby.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pulkxnuh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2tapxicls.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ysgqzvjz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ejnyzonq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hwpuawnd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2dltejwhh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2etehjpxk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xlbcewtf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2rifjsmwb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwhtdsc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kfunrnag.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iogpavhf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jtpkrxog.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkfroro.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vexjlbns.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2jsdxkrqz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gczgxqju.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bjvdgfyn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2yxlurhyu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2srupzgsm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2szblctna.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pxwkycbw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ujothmrd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xazuycdl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dsdrwvoy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kszaefzg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2dkatxmly.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ymervfhs.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2edpiykcg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lrfmzvzw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sglwioqu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2safykefk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ohdgqnya.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lfgrcqeq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cqpvpxqb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gznzviik.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bfeerfne.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ckdudepd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ugmkrukc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2uttcwelm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fbsymgxh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xfxbknlw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2spbeuppy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2maveeghl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fshttikn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ubnjzzci.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2twndvcbp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jzijowyq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xcwhpvnn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jvksiwmt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wqbkenqz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tutldddf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hzzywjar.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hrvngwyp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ekgieznt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hkjyaiar.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lvqhzidk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cybrrbet.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tpureoxc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ornfypfc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kpiplvdx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nbohigqx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oxbqwvgu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2btakuvyk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wrwtcxbk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2sysmckdm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rtgmoqhe.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pqijrdzl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wedkhnsf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ifencjyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsggofuh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dpmrozqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qviipurm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2wllujpwj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vexsjgsf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ddpscbjf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2aqmoubej.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zctgrvxi.html


<!-- 参考信息 -->