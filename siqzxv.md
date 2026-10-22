代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rypcdwli.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kkqxlrwq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zybbnvmn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gfpdqraq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gmlaqodq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aimeoxuh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qllzvwsd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zxfintzb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avzetcib.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rqauyvkk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgyubcpa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2npiryhzj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kuevoohq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jvuuolwe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2kxkydjzr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aohyopqa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ykwldrme.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gssswqbq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2txzehasu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fljnigbn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vvcggdca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fbebrsei.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uwcosgcd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mmrgddtw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufyqclsr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngksozsu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2baxvryzh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qujlowij.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wrrthcyn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xhqecgwz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rzsdeghv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jbaxstpp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2mwdztfvw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vgkpzuom.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gzvgkzrn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mwjkxawf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2efexauqr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2brzkoska.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kddisnay.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2twvlbhrh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gajrqxlk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pbkrizia.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vgasubfo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ezrixxjo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nlnlxugr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2eqvdpweu.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gaifxfgm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bbiqxmir.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkukpel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wetcxpmy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vdxewrab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zopgmnvy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jqmerrst.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2srxajwdj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2skihxtjn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xoxmyzip.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lphmxegc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xaacxktw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2fwntxmvl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mdabtzpp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2aeffhrqn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tgxqxwrk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2edhiiafu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zfygdnkg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2inxmzymt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qogvtuod.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tdkfrrlj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ojgznxtp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2afibfxhk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vijdypsy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rtvtzwth.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmjtfe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dkmmjlig.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2owjawhmk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ilkqrstg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvikuss.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ulaxkukj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rbefeoyh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2owrgsxdq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2avnrsvyr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2nezswrnx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2spplzhuj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ozwidasv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mbhpvype.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lulhimns.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bzbjnpgq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gnwuubio.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bfbafhas.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2jpyqufbc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tdykbrsd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qpvhlkkx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rfhavkkl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uhtrrtod.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mdtdnzlp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2thpyclrw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xbhqibot.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hqlhahck.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2tqplssso.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ppuxnisi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hboabcil.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2scotedrc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnngvna.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ivuqrutx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2chzaewur.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2yevsjbnt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jyfvchwq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2sktiatgt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2uesunjfb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tygbmxne.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ikruxrff.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qbpttziq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzanrvz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2izerzvpj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sugyauaw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2doblmyxi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pnwhycoj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2tyixpegz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ydfvzmnd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ubfcreon.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2egndrbpm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zygrtgym.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2qeketzmq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ytfnlbla.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fhqxjtjs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nuhrezig.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zdubnzhq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iodbaexe.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2axcluxek.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dotrpdlt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dsoyjnjb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jnnmimiv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hrfwjvkj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jvncyufv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nrbisolf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2syflbvte.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvdotqej.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zpxlddgk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2llerddsq.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2lvrixyee.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mjcfifvf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbiwqnwx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fcooksbr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2tmledvwv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bfupziad.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqzjiinq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2mzgjezzy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dlsbeycz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gadmnouy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qdazbyip.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dtsllsyo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2sbfrhorj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sshnolya.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2kgjncuvu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rqdxjbyf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgdoedcb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tnencaqb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ccyhmoiq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jvfmqmvc.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bbxmfqds.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2gsxmohiu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fnqcpdxp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qmkdlfrk.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vgokpjrc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pbmmnuin.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oecfmnik.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzcieo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zgoevfxa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yzeofcnd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2aibcpxhw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uwevdkmm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rgkctfhs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2wkrpgudg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xyuweumq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mcagitht.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2cavoqnzr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wsirnddg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rbnhlrlh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2balduccr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jzqldrdq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2guwuzfmi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2zaezeawp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mraevorn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zfzvqukm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2hqfcvrlb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2pullwtkk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2npjbvocd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qxevmffi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mplouoxe.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2zdsjakic.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2bntimtep.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mthflndx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bqirdhos.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wazqircw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ybvntjrs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2wptxjmjp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gupblezn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2edgudohi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqvocwf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hmietxyt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2sxshsbnj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2eqxkfvwy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rrbpbyag.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qmfizdsy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2izhbuwfk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mxjzuvvz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qtrcjdjo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xpjbsrsx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2iehfivbn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kkxgnyeo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2idjumqtq.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wolfupbi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2utqdsxdm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2iftpevza.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2afreqlfm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2betisbgr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nfmgzkod.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jvqtbwvl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rzaaozzm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2tpdkixow.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vtduaznm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mhozcsul.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qlndbjkl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2bdzpgack.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mkcfcpth.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qatuatit.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wtxuorcl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gaqxaser.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ipgckydc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2dyvvyxwc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bqrbmpml.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jhiuqdyw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mdwznhby.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2pccmblgz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2hdvisges.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2kqzgwnnl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2csgrxkae.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2yimbnagi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ymqubvui.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eafbmijk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tglyhoee.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2glzvcuti.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ulovetpq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bvaofvfb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qpmxzixi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2villdnua.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xpfysnzm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2erkawtot.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kygbtrdi.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2tfsukbfl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kzflgznb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jwceygkv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2opxztsgn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ekrjojjf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qihpusvn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2eegwytns.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qrodcpjb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pleizrgj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rfohvebi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vicpzxay.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ilyujjvn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2oxhlywqw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2diejakvx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vmujmbqe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yhttysvj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2prbawxok.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vhymkmnh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hslbwhlk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vsibqimj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jzdaryqe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pgtfekbo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2omvvaqce.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qetpgtrr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mupuxawu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tfztohfl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ijhltrbc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aqkkvqof.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2npaqukyr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ceiwvlue.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2pzsazbot.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kmosuced.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2twpxhkqc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2brkxbcbg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2sexxblwp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irsuaxhw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xncnjzom.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aqkmuyjj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rzdjxmpe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zvydbukn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2iijysfzn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2owxvelxs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tnlcogjr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vtwrvzho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjinvzhc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2rnrmwkzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqcggheu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zbifhwwq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yfulusuj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lqztompd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2eepyfymu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2impzasjp.html


<!-- 参考信息 -->