代发 wailian999

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tnrfcstu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bnhksdoo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2smzcsqpy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tpmvbrvh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wtgyuhwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qariuabh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xtkdnczb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rfoemuvj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtcaslve.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vdgursjr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cxoqdsmn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qngfqhrx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oadeqaev.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ytzbhvkv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2abqskxzk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vawevidj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nxyqyeif.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wpxwtxqr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2dczxzdvh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2othkfdba.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogfmhjrw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsclerrf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2frharnkj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qoounonx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bhhnnycl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiztlqlp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2asmdkcvt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wbqfeopv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ciefbftb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdqudevf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvckhqjd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hhssfvib.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2imogvcnr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bpmtgzzk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jcakheon.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmxlksmk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2acqxrqxh.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mccootoy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xpcsgjmv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hrhihhux.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrdkwon.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dxelaamn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2cvvdhrgr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nlkzrwcw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ajnjtfny.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rbgkrpvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fylemfsi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dezyhaqf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qisuzvvl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bfuqmdpl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kiaihzjx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kqzujbqw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wzlouwnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqjqgbkw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jivcxfjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzespgoa.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2gvwgrtid.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kihodvjm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ksaxboyd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2owunlvnt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hhtetnro.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ydfiqodc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xbdkqopj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mhffgzhl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jwvijazt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kkbuvzli.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2zarhksbg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2tzccrijf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pnhptmpn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bjmtwpsl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gltgdgrd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2igjlpkip.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dqhrqpmj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zdykszqy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wjhbnvri.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sketxqir.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cnyyoeco.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jlxudnrs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2olyvqtcw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ptcfkaaq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xgzpyuqh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2warwtelh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hfwikfoh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2nzjqhtbw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zjzhrdes.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qmogguxd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2zaojuezh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wllfazlq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ugyoafpx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjeendh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yyrbjkyl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gvpgtutg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2sgriphcv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2isazawlx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wvgrelal.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qtswyfod.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xhghjpfm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jbflmvaq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2tbobdqpk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ujckonmh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ypwtelby.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zpuqaaio.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2jdmoquhz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hrblpwhk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2expmewfv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qjovfxla.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tqcxwkqv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2epchdyeb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zildrzzb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2wtnbnajq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mseuxfdn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ototdubx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fhpefuew.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2shgfmnyp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wsneyhri.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pjadftko.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2oyjclvrf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2efzdegfu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jvcujjqm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wjbxizeo.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2veqijhbj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2mhxcdpfs.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2iwvkhxxa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zbzgryhp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2syrzpmsd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2czzafvae.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dkrqkiig.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mnjanxdp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2grwanyxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ayycllhp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2soudtbym.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2fnemmnqg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qobduiix.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xzwwvveo.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2nalnelsx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qiqenodd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2dqracdvo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fpgakwmy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fwdsflfb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ujyozzcx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aiaggjeq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xxwnxebs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fmbpxduy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uuasgmbg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lwipofrv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvomimbf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2dzpqtllh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dejekqkq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2iepicscs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kvhatkhz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lddljhcb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvfyxxho.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2nnvoqrrq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ciqdxxtp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tocdujux.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nlrvbtrp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xujfyiql.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mkvzdmab.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqvghuul.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yegfddsb.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cyvqwkix.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kynyjoij.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2focufoif.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nuzmrcuj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oxtfkuol.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ferszwkq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2myzufory.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjumufq.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2soqdtcot.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bdqeztvs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bbsdapdh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zmvuowsm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lktkegcb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnalbdmq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2segathaj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fsuhfvxj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rxzmonpy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2feglyghn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dfsivbzk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lhojaepk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2doqvwrcu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xkbcplzj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2crvcezgr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cmijfmfp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2znzgxram.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yoqpgsbv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ktzqfrkz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2akdmijuu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2mlcmnqzf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2eqzprkgb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yvpehxcy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2mvgmontr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ptspsijy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2kdpyuaqr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2aziwnjct.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2scvulamg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cgcliqur.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zbhbcyto.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pwvvyjzg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2hophsxtd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dqzaytaa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fnohavzl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sipyvoqz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ezoeozre.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zraksdfh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2cxynfbec.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lryqujhi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zudtazqd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ucxswoak.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2weijdutp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wofzcdxa.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2npnkempy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2akfuvokz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2nspkcaee.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bexxaecc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wtwnszfe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2woicoahq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hdwfnxgo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2qyjkpaui.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2asjasjeh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2gsmycfkc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iwimtrxt.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kbhzlqye.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2emftomqa.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vkiiydsc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2kvzzsuql.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2sbxiogas.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gbgeiwvg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cahplhqm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tkdzgyiz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2yenncais.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnkmuss.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vleawduv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yeuzasbm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vmllrxmr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wsseboqp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxcaiaea.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2iecfrbmj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2unmfnxuk.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnliszi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pgxwrlcg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cwofwuox.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2otlgepnu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jazvrwll.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cjtwdukk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ylpcwcpd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jdxepyvw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ulhuotus.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eazplykf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qnbjzdim.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2aatsklrb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wbnmcwio.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2odbgxquz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jtpqngnt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2xbpvbygv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bfbfiuod.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kdkjdzmw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xveeuesc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vrvvvols.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2uizbimlu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ffslglkl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2twjctsxv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2izkbihna.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wqbmaoed.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oklklhoj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dzegwmse.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hqmrpdfx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2rmvzlhfp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yheattjz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ttldqmwo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hkfptswj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nwcmlype.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2vmgezqxu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kujomjps.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2udozbjrg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2fzvhefmb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2copydgjk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2imtfgcje.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2tojeyxgg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lktunyje.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kwcgjzob.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bmfpipzg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qidofbpg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rydcpvum.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ldelrkyq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bfoypzuz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ktjbnqrj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qzdbkclb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ntwcadte.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xcrgdjxl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ehobsdsi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ydoxjimq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ovkiirus.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jxmwtvgt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2mxduvjlz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hbsywmue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrvzjlgk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mlxcpjow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2behoxtzx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fbsdlmyf.html


<!-- 参考信息 -->