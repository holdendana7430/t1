代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cmwbeghw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aimzhgyy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nxneqnfk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wroejqkx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvrdmffo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2crtjbrmq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyrvcwth.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ojoxxbbl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bacsgeoh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wciasglx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2hltwxuoo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eebvquoj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrkcocir.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2erxeocel.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejkqybtj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljagegmy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2eejshyml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bamnfjto.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2klldbhkv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qlzozxlm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nmvgobar.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2htirnyzm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzsoaoct.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rurxjlbl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2adxlzrrj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jdmzspbe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2asabwogn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sezcqacv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lgscntxt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zvjhjekq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fbfxnzby.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kgepoxef.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jeegwyxk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rrhtejeo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ykwewtpm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gddqllcd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgiwkyt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvkxwo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hvmdkicq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xzxnfpeh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qdhbkual.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2naythaqo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmlfmkv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lvghfnxf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2gabfjfij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aslhshhn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zhjldkgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loqvqkcx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2umtpuylc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bhrgxvdp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qckaucxb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhxovpyw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ksdbzkqy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dieojgqh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nwguymtw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jziwicqc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ohifcrmi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2chsdcgwu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uihkccgf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2jucivfky.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lucbqvar.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oeqcwxlm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gvkaeuxl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2amrymasg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bzhmlgoi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qocyoanm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lubhypxw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fbbfkige.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2efzfvwvh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goakjvck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wpzpswfo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhrfsecb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxtdnywv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ecmipksv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2osmlinot.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2glzqxvkd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2izucjiuw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ztolbxbz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2uagxykgh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jmyrlgim.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zruemqua.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nubxlpwc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xfspsgiw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lxcdjjhx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2niknaeak.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2aliflodq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2mvtkneeg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gbtxkniv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2puitinlb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2obyclmum.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zdmudpif.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gzmzwmhv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkkkiggq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qvajtnjt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ihgsdkkx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sypgycwt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qgzepkfx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ibugfiyo.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wbvvcqvr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pwarqkfs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ozycpvjk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tcgdswtp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tptsykkx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kmoonchx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fdvfuyli.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2focvrriq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sgppjebx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2taicegty.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zxabsjlo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2tjkdohsr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2attqcavj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2orvhwxhk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tawiquwx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xjsfdyfe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ggpmkvyh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2osmyzmyb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xbzlpuwr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hzpcdozq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rcbbdnbl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2xnyignoa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ewfrhncu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2yddkjhdv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qpwjhusg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sqonyqas.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2uxuzwnma.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wimebxym.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pinfswbh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqndaqg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2clefnajc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fnjosnju.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2hzymvjpp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2dfflrbmz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2uoarrflf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xmksvaes.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2unfensrc.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ojddzqit.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzjhzsou.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jlzyqnra.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2vrofyppb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2zvzcowsh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2smrxlfnl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zbjdppmw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2immyipdw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oajprlsz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2tmlprgli.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2hwbifuoe.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2hkjfvegr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2luwrnpaa.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2vodohruz.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2vnmpwgha.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2awypdudr.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mzqrexgv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hqtcnxdw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2uzbocvgv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2dxdacuuf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2tcqqrvho.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yxrcdepv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ekvmrjiv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cmtjgxgq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2elynfmrh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ccbquvcp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wawulbds.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2lupkbvwv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hyywmixk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2yolhwtdp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tbpwzufi.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kljftmql.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2sptjxlfb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kzkayydz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqpraodk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lndenofn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gdljsbgg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ernxwtob.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cktbplse.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzcbrnnx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qsrjfotk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ezytlrbw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yldoqgxm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jshivejc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfoecbnw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2hpytnusu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2dvfkpved.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mqgasoca.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2btynhamw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ipwjkfpz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tmpyzimc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2obzuhaip.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kaqcagij.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wvrccryz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hymfrjoi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2avhmqpyr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2obwumcgo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2rtoqeaxb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2txcgfebv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajpflcwc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2vctcciqy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tcialwfe.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hllqapno.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2mormfjtx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2vyvvscux.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pddfqcdx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2cijfuntw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zuodclrl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ypgcnfwl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qwzvgztq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ewisvrut.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xbtmeswr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2xtzewzmf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2oturkswl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2txxzbbwq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mttuzykk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2kstyhcsd.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fhpoxkbo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bapbreel.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qrwpbjso.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qkufxrtv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fbfivqxy.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hrlxylkf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2awpovbyy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hbxcwdur.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vixrsypt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fbmcpeky.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2sklzluci.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dronufdt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cqywcnbl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nnkbcria.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ssljibfq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tkczhgkk.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hxszalrz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2cdrwpfmu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2udyjzypd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwscrwn.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwbmjsjq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lljpeesr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xbguaswp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uirvbtwe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hzmgbfii.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ycyrccel.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kgkehfiy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2otilvbpy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ckdstril.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fgfkrhhg.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kdetlecs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gnynitwd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cpbsxgyw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aaylokkk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2owbssmmi.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2prvkqzol.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ltupeiou.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2whriucsz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rxkalvxm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2arwqmpoh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2dhoncywc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hydgdlcr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yyaxdjld.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kzyuhqnx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2yzrksmrp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zirzlhya.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zvritvqs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2bexpmeje.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dsezurzr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jsftzpop.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xupvwwwi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2luvctptv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pmtvzmej.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2xxsiuhig.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tuvedkht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xzrdgdmg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvtnia.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2acqngdej.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2khoevkhp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ieworery.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2sxvmkura.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gkajahhn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2cegqmxih.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ywjocokf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ytrccwww.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yiegyect.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ytfoecnx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brnvyjqd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2teycparu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dayteseu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ipcescfi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pdpeycfe.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xaggwqhl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uiehdgqx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2sybomxnf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xvplavlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgqktfro.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xqmqztnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wditdrum.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nzuyaktk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qtudqrnu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2psrwfasx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cxbxgrcj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kqwrvinn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ttsoqaoz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2acrgjbdy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2cbffpbjn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2gcdweiqf.html


<!-- 参考信息 -->