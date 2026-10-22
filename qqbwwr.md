代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2szkhmyqr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wbdvlkok.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2exgwbjlu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jnwoypoe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qrlygkht.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rmcwsxsx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mjjthlvf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nqfpkphd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cizslpzl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ulgmnbck.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibmmccuz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ifyzxfwo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2esxezoqf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jilncxzr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oxsvzpav.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwwqoeni.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dxvcrkfl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqioqvmk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mztuwecs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rebgtgxb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xwqiotvr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xfddgmtf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yemktpoa.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hambspfu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2resuzkrn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wijwsksf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kgzayopy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yzbjwzon.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjciiwj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctnkmvay.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zvijpjjm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ikraphmx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cqueaidk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wiptvynp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eyoacvqf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dmmtliar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rbghliid.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xneiymgy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fijztmfw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2govlretw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjtblrw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fhbvvxcy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2niujwsuo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xlxuqjiv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fxnkhwqu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2thqeogpk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wwribpbi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2cnvcrati.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nvrdtnef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzghshbn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kvvaonhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqqpnyiz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ubtqsvpy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2aifwxrtq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2sozxqfrm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chssfunn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bvnpuusx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vysitcua.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rnasntbk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yrlaqyhq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ztvsthla.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nxljfpzb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ddhtcvxm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yekmnmwo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vsvjjzek.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bdnsuaqo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xrbaogle.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rovmxrlb.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2eorhhdev.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hgxbqqin.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wosviybf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lypqmpvh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2uavvpojl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwrdlqjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2fxvgdmyc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bavfdlin.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ycacortr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwepyhc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yyifxvmd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fxlinstm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uygvadtg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uwtzlymr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2csbqeyxa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gmchkaen.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gmizvhfo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2szluwrxi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fjyoehix.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mjlmfgph.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ivtwvxxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2eyjmbyhd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2npihhupa.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2vgqqzhnd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wbnpqdlr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2buxnabpi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2exdrvqfi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xoqqqqpm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lheohqjw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fbzxtska.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2dqupsvyp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ytcekcez.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2kricmlyy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ahxflkau.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2lntxzegw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvfdwio.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2xwfhlbml.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ojilhcxo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2njcxbqtd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dofdrqys.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2weteyecf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mxyqzbga.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kxrcoelj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bszprufr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2knogcjed.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nrmocwbc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2adppisnj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2abrvgnza.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vznisdou.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2wnshmgvi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ecrqudyq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2kvcotcbc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jdlvfwgd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2rvlrvwdx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vbvyghzj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhckbje.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2kyrvnhkz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2vbtxkzqs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nrxrxwsv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xdfcogyz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2yuybmpwb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uufpwpbg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2audajvwd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mtvsybqk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qbasxumx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ompxppdr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2dffinlyr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qehrktaw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rdumgsgy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iqniudev.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zklpnvlr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mfraondm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ahadxkuu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zcfkpghf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2wagkfrid.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vwbmdjbb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rrwupvrf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wjlojdwt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2evvtqfyu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2albqfppq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2sedwjpby.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2gqondmzj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zmzepmez.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibrujupu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2hgfctrut.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2lxisthft.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tcenlsvz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2amqwlqrm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2uzocgkgb.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hphsixgz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uplgiirs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hcncshms.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iaavabpz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mlpmtegl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2giqhbwwl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cerahnai.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yklrgtby.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kzvxcjyd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lekbgegs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2kwvmurhf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2owerhzvb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjqnikut.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dtojrybk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2luewfsiz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kcskggzs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wcblbebc.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rzfuukxh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ewrlsumb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hlnaopgg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pgvalcif.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2elbztdzo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2dxcylkmy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2txozddem.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pqlwdsud.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2szvmheot.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bhrvrpem.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2vuhpovsp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2matqlwwk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2awcakqat.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rawtxsex.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2sjuuuesq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bijuknjm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2qfuskzbm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ynkzuriz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ocreykhy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2joszujbe.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ssuljhbo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2fffnqmlg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oftiipyj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mnhftozs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hbhdhmvw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wdajmghl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iocvvhwa.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vivsrqva.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mkgvncgx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2byxnddqi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ylzcdzey.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xcwgyhdn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hwtqjapo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pnlbalok.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pbjlpdye.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2perleink.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dajktffd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rckghsxm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mnogdoyr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ukxmyrai.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2uduohgxu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xcpmylud.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ggymuilx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xqszdzcm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2feduuhzo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2oyehwgmo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2pvvolsag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kcsycexr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bloifggd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hjvnbxal.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oeydkzeg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zysmvgwh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2jkgtgiod.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2gtddgfpd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2kjpzirut.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2elujvwka.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2omplpdnt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkulfor.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogasghmd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jpszropv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wojirscx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2esklktho.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2anynkzum.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ogrgmpzv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xspdkiro.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kghcopvq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dgqroyjg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gutdwadm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mhmdezgk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jcaercwp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wutbyour.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qgaiwxcp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ooaeudod.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zfwsewvt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gkmkhyed.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2csdtmleu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2dywfhpda.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ydhjdcyo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sxyqxvkb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2fpekwmin.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vtxtfkmj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zdphuhbh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2iipprqyo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2bbzcvlps.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wvpyodnv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dontbwgy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mcpxnlrs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhqyaxit.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cpfdlqrq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fkezpbjo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lphiefsx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2srnpuewj.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mfatedvh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qeumjrjx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vqeeomjk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gldplvav.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2njelsbck.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vssuudqb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nlsitzfv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2klddyjka.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fkihhezb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oghrxxfw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kprhwqgm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aiqgehto.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2snodhopl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qklrllbr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gizclxgf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bomydgcv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2alihyddb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdxaujko.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rxrpsynt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mrnmpojj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2wvgeiepe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zanlwtuy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2cungazvz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2vghrcxog.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2lpqdfabu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ojfinyjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikafuvkd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dndcbboa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arqbaixp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rddfenfl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yzcsjhfj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2avgvkoxp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ibrfustm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2iibveytk.html


<!-- 参考信息 -->