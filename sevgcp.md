代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2knqyudhd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjeoqdm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2heoloarw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hkhvwfqm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2esscahkc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cupozxuv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nptuqoed.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qajlrszn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xfwqgqqk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qbbsuklb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qozzouvl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wdocspcb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ljxphwoy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnipxwed.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpqhrtpv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtblfzwx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xzvdtqgx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kmfmikoe.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fxgegzpg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xgiszivs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hxabpgko.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ifjuvrdq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2doznzpha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ikzpqtgj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iigrmngf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xxhxiaek.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mxsajnec.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pevfffzj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mwaeipwg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2udaksori.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2emwlqxmc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iazpwldf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2celnxezd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jrlwnotj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iddqrruj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nnxdlkja.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mdscqjox.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wfvkahok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eyutvvbr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ijazuacq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jzbskurd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ldqzmdpi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2smeyzyrx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hmgagyih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2exxywicd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpbrrysn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rmfkzmpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixedvtht.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yqwonmvu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ttnmcruu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tmigaltm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lbbvtwbl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mukkzgwl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oapztzgx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rdsdxoce.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hrimieyc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ozerfbfk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zysqaxrc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ewbrmcsn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zpptmrkj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pgwrhviq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oeagmlua.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ijclvxmn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2aszzfbwh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2lyqhdste.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wwhpbwmd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dcqptaqe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pprahpfr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gbxzznrl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jtjeghmb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zewnttau.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mzarzjsm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozgictld.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dzgjbxyf.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hrtvvypo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cijsjhgf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ogtbddsz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fxonucmg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2hrjridvp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dcezknzt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2mdhjxolf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ibhbxmvv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xrfsvluv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sdduhnlu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ekwgmisg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2huuqtwza.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2cqcjxgfy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lducxpsi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2cmykbtry.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2faslpuso.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yrccxaap.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jjyolvxz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkaxltoi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yinekwyp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vidxzhmv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ihlorqjp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iofrljvg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ocqfwuza.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xhcnlvuw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mgazzuag.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zikhbwwa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bipifiid.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2yhtcmbrj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2wasrwzmb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kzrfmvco.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wiodwbes.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aagokhdr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qmylvqvf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ofnmagzz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mgfkuiqq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2iwdsvbaj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fcfwkbae.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hxmmkmhl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nxcxvchq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2cnezsskw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bnmshjkh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2rqqbmlqr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdessbh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2lknbxval.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qgkjfkje.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ndkdnzyn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rxpmfxiq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2enrhunaq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dgokwzgv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xdlczadk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ixdykwym.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zfipvcit.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vyioafrr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2mzgxzhbg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pzhwfaop.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2koyaebng.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2xlxuacga.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2wmnqqups.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ojcimiba.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2jnbkazvt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ieetzeqy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2avzkzevj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfnfrvrm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2uckanjkl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2byqeavhr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2jertxjjh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ztwgwuiz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ttsjgmsg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2vwlrkgnv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xthgorjv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xdkthjph.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lmnikdsp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mudchmob.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2omyayvdj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2xxfcoekk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hlrutkun.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kdbunaex.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kbrehbft.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2odaqxnwa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2uebslvyh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pvimfcnc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tremzpmi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gqokhpeo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wagjcoqj.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mqdivnng.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2anugaqpe.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gvuddbop.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jxvnjmgc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2sbwoomnq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2cgemlnbe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2psamjvrs.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2dbgcypde.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hichetkq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xvwxtsiu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2odoogatb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2cworzniz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2sdqwqtfb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tmtbmwlc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eqlnuhcm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tzsyhypj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2xnezuhsk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kzychbsu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2szftkfpv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ueydhuoc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgqeepix.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2zkaxxjzd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2njpkvgvj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2bzshewfw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dngfuviv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vrumssuz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jqsthvnh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ciorytvw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2sqjdccml.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lczguplp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jmklrnck.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2blunjkdu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2knddyvcy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2reglodde.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ibhnbwnq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2plvfruuc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2eantlyqe.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2wridneqe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2zcuhenfl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ydwrsnzy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2huheecug.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2faspnimc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2uoopoaph.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ieeytdho.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dacdzkdu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2unkroahr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2xjywdpin.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ekmorkfm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vqihddom.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2ijpgkxju.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jdkphrxp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xgxqouti.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lqotcoaf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2oblmguly.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xjxrkcge.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lhrhujfj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lsfmhiyg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ywoclgzb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2veyytanq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2iimozvjj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2goxbxght.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yhsgwjqr.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pkvafybw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2oasbkzro.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2llallvlf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2onippxdr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2evvpwcvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2efprakka.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xhzsngxu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rppnzbit.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xzbicann.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qmlvvmai.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2whkpwoin.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2rlcellpr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xnspjump.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hspilzxr.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2clhwekvi.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wobgatsd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2clbikinq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xityccai.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wujuiihm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zrlrchah.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dqwikdvo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sdtfczdg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gghyhgdy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2alkikbqd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ykanljzg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mbvlsemd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nwoyuoxb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2hyoiyhxx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2wszpyyta.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iuyeqgco.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ussbtxhy.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2awfkpwgl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cynvnjsi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hsybefkt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gzcoiakb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2aoiyixfd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tntqjmvs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uarryuvy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2tfayyszz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ndhgqryq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2sckalryu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2aqoasbvk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ttxkletm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2oezlxwsz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oqeuptfk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ezflfxln.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sblubmcp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2eguknced.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cbtullsl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ctylbkfg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kegbkjqy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jlmzojdx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ahexlhzz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ayfuzowt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vnplgezc.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fdcxrnok.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mbsvekbd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pzvpqtws.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nchrfivw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lqwuvtix.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qzruaepa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2esqgnvau.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rytvkhuy.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vixgkwwb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lkuilcfd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ypzzkrai.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2brvlzzoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nscqxjga.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pbibhrwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmtomfqa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2juejpkmu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rciimqph.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uiptjxev.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2agpawocr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bqnovxkr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xswljzif.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qustvaba.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xphznkgs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jixhdzaz.html


<!-- 参考信息 -->